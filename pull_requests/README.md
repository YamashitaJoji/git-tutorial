# Pull Requests (PR) -- Contributing to Others' Repositories

A pull request (PR) is a way to propose changes to a repository on GitHub. It allows you to notify repository maintainers about changes you've made in your forked repository, so they can review and potentially merge those changes into the original repository.

## Adding yourself into the hall_fame.md

1. check out to the `v1.0` tag:

    ``` bash
    git fetch --tags upstream
    git checkout v1.0
    ```

2. create and switch to a new branch called `hall-fame`:

    ``` bash
    git checkout -b hall-fame
    ```

3. Open the [hall fame](./hall_fame.md) file in a text editor, and add a new row in the table with your GitHub avatar, username, and a brief introduction about yourself following the existing format.

4. Save the changes to the `hall_fame.md` file and commit them:

    ``` bash
    git add .
    git commit -m "Added {YOUR NAME} to the hall of fame"
    ```

5. Push the changes to your forked repository:

    ``` bash
    git push origin hall-fame
    ```

6. Go to the original repository on GitHub, and you should see a prompt to create a pull request for the `hall-fame` branch. Click on "Compare & pull request".

7. In the pull request description, provide a brief explanation of the changes you made (e.g., "Added my name to the hall of fame") and submit the pull request.

8. Wait for the repository maintainers to review your pull request. They may provide feedback or request changes before merging it into the main repository.

:tada: Congratulations! You have successfully created a pull request to contribute to another repository on GitHub.