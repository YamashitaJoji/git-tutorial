## git branch & checkout

:flags: When you want to create a new feature or fix a bug, it's better to create a separate branch. You can switch between branches freely without affecting the main codebase.

1. check the current branch you are on:

    ``` bash
    git branch -a
    ```

   > The asterisk (*) indicates the branch you are currently on.

2. Create a new branch called `feature`:

    ``` bash
    git branch feature
    ```

3. Switch to the `feature` branch:

    ``` bash
    git checkout feature
    ```

    > Or you can create and switch to a new branch in one command:
    `git checkout -b feature`

4. Add a new line like `This line is added in feature branch.` to the README.md file and save it.

    ``` 
   
    ```

5. Add and commit the changes in the `feature` branch:

    ``` bash
    git add .
    git commit -m "Added a line in feature branch"
    ```

6. Switch back to the `master` branch:

    ``` bash
    git checkout master
    ```

    The changes you made in the `feature` branch :arrow_up: will not be present in the `master` branch. 

7. Switch back to the `feature` branch to see your changes:

    ``` bash
    git checkout feature
    ```

    The line you added earlier should come back.

8. You can also push your branch to the remote repository:

    ``` bash
    git push -u origin feature
    ```

## git checkout

`git checkout` is a really useful command that allows you to switch between branches or even revert to previous commits.

You can checkout to a specific commit by its hash.

1. check the commit history to find the commit hash you want to checkout to:

    ``` bash
    git log
    ```

    > You will see a list of commits with their hashes, author, date, and message. Copy the hash of the commit you want to switch to.

2. copy the 4-5 charaters of commit hash (e.g., `ac9862`) and run:

    ``` bash
    git checkout ac98625
    ```

    > This will put your repository in a "detached HEAD" state, meaning you are not on any branch. You can look around, but if you make new commits, they won't belong to any branch.

3. To go back to the latest commit on the `feature` branch, run:

    ``` bash
    git checkout feature
    ```

    or go back to the previous branch you were on:

    ``` bash
    git checkout -
    ```

:tada: Great job! You have successfully created and switched between branches in your Git repository.