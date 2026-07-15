## git add & commit

In this section, we will learn how to add files what you have modified to the staging area and commit them to your local repository.

1. Adding a new line and text anything to the box below and save the file.
For example, you can add the following line: `This is added new content.`

    ``` 
    
    ```

2. Open your terminal and navigate to the directory of your cloned repository.

    ``` bash
    git add .
    ```

3. Commit the changes with a descriptive message.

    ``` bash
    git commit -m "First commit: added new content to README.md"
    ```

    > Committing is like taking a snapshot of your changes. The `-m` flag allows you to add a message describing what changes you made. You should write meaningful commit messages to help you and others understand the history of changes.

4. Now, all of you changes are committed which means they are safety saved in your local repository, and you can look back at them anytime.

## Going back to previous commits

Let's try to go ahead and see the previous commits in your repository.

``` bash
git checkout HEAD~1
```

> We will explain *checkout* in later sections, but for now, this command allows you to switch to a specific commit. `HEAD~1` refers to the commit just before the latest one.

After running the above command, you will find that the content :arrow_up: you just added is no longer there because you have switched to the previous commit.

To return to the latest commit, run:

``` bash
git checkout master
```

:tada: Great job! You have successfully added and committed changes to your local Git repository.
