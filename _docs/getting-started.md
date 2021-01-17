---
title: Getting Started
description: Getting Started 
---

# How to contribute to Docker Community Site

This page is intended for people who want to contribute content to this Docker Community repository docs and who don't use Git or GitHub often. The page is basically a quick guide to get going with a GitHub repository, using either Git on CLI or the GitHub web user interface (UI).

## Using the command line


1. Fork/Clone the docker-community-leaders/community repository:

    * Go to the [docker-community-leaders/community](https://github.com/docker-community-leaders/community) on GitHub.
    * Click **Fork** to make your own copy of the repository. GitHub creates a 
      copy at `https://github.com/<your-github-username>/community`.

2. Open a terminal on your local machine.

3. Clone your forked repository, to copy the files down to your local machine.
  This example creates a directory called `community` and uses SSH cloning to
  download the files:

    ```
    mkdir community
    cd community/
    git clone git@github.com:<your-github-username>/community.git
    cd community/
    ```

1. Add the upstream repository as a Git remote repository:

    ```
    git remote add upstream https://github.com/docker-community-leaders/community.git
    ```

1. Check your remotes:

    ```
    git remote -vv
    ```

    You should have 2 remote repositories:

      -  `origin` - points to your own fork of the repository on gitHub -
         that is, the one you cloned your local repository from.
      -  `upstream` - points to the actual repository on gitHub.

1. Create a branch. In this example, replace `documentupdates` with any branch name
  you like. Choose a branch name that helps you recognize the updates you plan
  to make in that branch:

    ```
    git checkout -b documentupdates
    ```

1. Add and edit the files as you like. The doc pages are in the
  `/community/content/docs/` directory.

1. Run `git status` at any time, to check the status of your local files.
  Git tells you which files need adding or committing to your local repository.

1. Commit your updated files to your local Git repository. Example commit:

    ```
    git commit -a -m "Fixed some doc errors."
    ```

    Or:

    ```
    git add add-this-doc.md
    git commit -a -m "Added a shiny new doc."
    ```

1. Push from your branch (for example, `updates`) to **the relevant branch
  on your fork on GitHub:**

    ```
    git checkout documentupdates
    git push origin documentsupdates
    ```

1. When you're ready to start the review process, create a pull request (PR)
  **in the branch** on **your fork** on the GitHub UI, based on the above push.
  The PR is auto-sent to the upstream repository - that is, the one you forked 
  from.

1. If you need to change the files in your PR, continue changing them
  locally in the same branch, then push them again in the same way. GitHub
  automatically sends them through to the same PR on the upstream repository!

1. **Hint:** If you're authenticating to GitHub via SSH, use `ssh-add` to add
  your SSH key passphrase to the managing agent, so that you don't have to
  keep authenticating to GitHub. You need to do this again after every reboot.



