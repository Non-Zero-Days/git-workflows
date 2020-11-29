# Git Workflows

## Prerequisites:
- Install [Git SCM](https://git-scm.com/downloads)
- Install [GitHub CLI](https://cli.github.com/)

## Loose Agenda:
- Gain familiarity with basic workflows in Git and GitHub
- Identify difference between Git and GitHub

## GitHub Portal Step by Step

### Create a repository

Open and log into [GitHub](https://github.com/)

Click the green "New" button on the main screen

Note the options including settings like public and private

Enter the repository name Git-Workflows then click the green button labeled Create Repositories

### Clone a repository

In a terminal, change directory to where you wish to put the newly created git repository then enter the following command

```
git clone PUT-LINK-HERE
```

Note - you can find the link by opening the newly created repository in your internet browser and clicking the green Code button near the top of the page. There is a clipboard icon which will copy the link for you.

### Commit to Main

Add a text file into the cloned repository and run the following commands

```
git add .
git commit -m "Initial Commit"
git push origin main
```

### Commit to Branch

Add another text file into the cloned repository and run the following commands

```
git checkout -B nonzerodays-branch
git add .
git commit -m "Initial Commit"
git push origin nonzerodays-branch
```

### Create a Pull Request

Open the newly created repository in an internet browser

Click the Code tab at the top left

Click the '2 branches' link above the list of repository contents

Click to create a Pull Request

Enter the title "Added text file" and body "It's a non-zero text file" then click to create the pull request

### Merge a Pull Request

Open the GitHub repository in an internet browser

Click the Pull requests tab

Review the files changed

Approve the changes and select Squash and Merge

Typically, I delete the branch after completing a pull request. 

### Fork a repository

In an internet browser, open https://github.com/BoredTweak/Redis

At the top right of the page, click Fork.

If prompted, select a destination for the fork.


This will create a remote forked repository within your user context as well as clone the repository locally. 

### Merge a Fork

Make a simple change to the repository (e.g. - add a space to the .gitignore)

Open the page for the forked repository created in the previous steps. 

Click the link above the list of files labeled "Pull request"

Observe the changes in the comparison tool then click the green "Create pull request" button.

From here, the experience is the same as merging a pull request within a repository.

Congratulations on a non-zero day!
