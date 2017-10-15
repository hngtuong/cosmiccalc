# Contributing Guide

## Important Resources
- [Wiki](https://github.com/blead/cosmiccalc/wiki)
- [Japanese CosmiCalc](http://www17.atpages.jp/cosmicalc/code-web/)
- [Cosmic Break Fan Forum thread](http://www.cosmicbreakfanforum.com/t15375-#353114)

## General Information


## How to contribute

### Getting Started
If you are familiar with Git and GitHub, you may skip this section.

Make sure [you have git installed](https://help.github.com/articles/set-up-git/).

Note that there is a user-friendly GUI client [GitHub Desktop](https://help.github.com/desktop/guides/getting-started-with-github-desktop/) as well if you don't want to use the command line.

Since there is already [an official guide using GitHub Desktop](https://guides.github.com/activities/forking/).
I will provide only commands here to help those not using the GUI client.
The process should be similar so you can compare it step-by-step.

#### Glossary
- **Repository**: A _repository_ contains all of the project files, information, documentations, and also each file's revision history. Simply imagine it as the project's folder.
- **Fork**: A personal copy of a repository. You can freely make changes to your own _fork_ without affecting the main repository.
- **Clone**: A copy of a repository which lives on your computer instead of online. We use Git to track changes and sync between your local _clone_ and the online repository.
- **Commit**: A _commit_ is an individual change made to a file (or a set of files). It is similar to saving a file, but instead of just saving, Git creates a unique ID to help you keep track of each "revision" of the project.
- **Pull Request**: To submit the changes (or to be precise, _commits_) you've made on your fork to the main repository, you create a _Pull Request_. This shows us the difference between your fork and the main repository.
- **Merge**: Once your pull request is approved, changes made in your fork will be _merged_ into the main repository.

#### Fork this repository
Make sure you are signed in. Click the **Fork** button on the top-right corner of this repository.

The forked repository will be under your name. For example, if your username is `manimo`, your fork will be at `https://github.com/manimo/cosmiccalc/`

#### Clone your fork
On your fork, click the **Clone** button and copy the url.

In the command line, run the following command:

```sh
git clone <fork-url>
```

For example, if the copied url is `https://github.com/manimo/cosmiccalc.git`:

```sh
git clone https://github.com/manimo/cosmiccalc.git
```

This will create a new directory named `cosmiccalc/` under your current one. It contains the exact copy of this project.

#### Make and commit your changes
Simply edit the files to your liking. You can test if things work properly by opening `index.html` in your browser.

(Note: does not work on Chrome because it prevents loading local files for security reasons.)

After you are done. Open the command line inside the project directory (`cosmiccalc/`) and try this command:

```sh
git status
```

This will show you if any files have been changed. You can review what you did and make sure everything is correct.

If you are satisfied with the changes, **commit** your changes with the following commands:

```sh
git add .
git commit -m "write what you did here"
```

In the commit message (`"write what you did here"`), you can write anything as a note about the changes made in the commit.

After creating a commit, running `git status` will tell you that the directory is clean, meaning that no changes have been made after your latest commit.

#### Push your changes to GitHub
Time to sync up your clone with your online repository! If you run `git status`, it will tell you that you are _ahead_.
This simply means that your local clone has commits which are not on GitHub.

Simply run:

```sh
git push origin master
```

Your forked repository is now in sync with your local clone.
