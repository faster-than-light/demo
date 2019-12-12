# BugCatcher GitHub Action Demo


## Setting Up

Getting the GitHub action configured and running is rather simple. You will find your <code>BUGCATCHER_TOKEN</code> in the dashboard of your [BugCatcher](https://bugcatcher.fasterthanlight.dev) account along with brief instructions. Click the "Set Up the GitHub Action" button to set up GitHub Action integration.

![img](img/setup.png)


## Saving Your Token as a GitHub Secret

Go to the Settings tab of your repository on GitHub. You will see a `Secrets` section on the left. You can securely store your <code>BUGCATCHER_TOKEN</code> here. &nbsp; *([more info](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/virtual-environments-for-github-hosted-runners#creating-and-using-secrets-encrypted-variables))*

![img](img/secret.png)


## Adding the GitHub Action YML File

GitHub Actions are triggered when a `.yml` or `.yaml` file is found in the `.github/workflows` directory of your repository. You can create a file like `.github/workflows/bugcatcher.yml` in your repository and GitHub will run the Action each time code is pushed. *(In our example we use `push` as the event, but you can customize the workflow yourself by using the [workflow syntax](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/workflow-syntax-for-github-actions) from GitHub.)*

![img](img/yaml.png)


## GitHub Workflows and Action Output

Now that GitHub is configured to run the BugCatcher Action on any `push` event, we can watch it in "action" by viewing the Actions tab on the repository webpage or in your pull request conversation view. 

### Pull Request Conversation View

#### Checks

*INIT*
![img](img/init.png)

*IN PROGRESS*
![img](img/in_progress.png)

*COMPLETE*
![img](img/complete.png)

### Actions Tab

*WORKFLOWS*
![img](img/actions.png)

*ACTION LOGS*
![img](img/github_check.png)

## Test Results
![img](img/bc_results.png)

&nbsp;

&nbsp;

<hr />

## Videos

### GitHub Pull Request Checks

This is brief look at the BugCatcher GitHub Action at work.

[![Alt text](https://img.youtube.com/vi/tsVAXfNqLqQ/0.jpg)](https://www.youtube.com/watch?v=tsVAXfNqLqQ)
