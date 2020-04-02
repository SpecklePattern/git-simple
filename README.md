# Simple git extensions

This project provides the absolute minimal scripts to work with git on command line. The aim is to simplify the git commands for simple git projects.

## Requirements

* Git installed on your machine
* A git account (GitHub, Bitbucket, etc.)

## Installing

Requires sudo privileges.

Create a new folder (folder name is not important) and execute the following commands 

```
git clone https://github.com/SpecklePattern/git-extensions
cd git-extensions
chmod 755 install
sudo ./install
```

This will make all of the extension commands (see Command reference) available.

## Working with a git repository

Here we will cover the basic usage of these simple extensions on a real git repository.

Simplest way to create a reposity is through the web service.

### Github

1. **GitHub web page** : Go to your account
1. **GitHub web page** : On the frontpage you see the "Repositories" tab. Click on that.
1. **GitHub web page** : Then you should see the green "New" button. This will allow you to create a new git repository
1. **GitHub web page** : Fill the Repository Name. Use name "git-simple-test" to test and follow these instructions
1. **GitHub web page** : Click "Create Repository"
1. **GitHub web page** : Now you can see the instructions to initialize the repository on your machine
	* If you just followed these instructions, you should follow the commands that include the command "git init"
1. **Your computer** :  Remember to create a new folder for the test project on your machine and follow the instructions on the GitHub web page.
1. **Your computer** :After this, you can, for example, insert a new file inside your test folder
	* It is important to note, that git follows changes. So, if you are not changing anything in your folder, git is not doing anything. Go ahead, try putting a random cat picture inside your folder and then continue these instructions.
1. **Your computer** : After changing or adding any files in your git folder you can call commands
```
git-commit "My comment"
git-push master
```
1. **GitHub web page** : The git-push command requires authentication, but after this, you should see your file changes in GitHub web page

## 'git' command is not working

To use git, you need to install the packages this is dependent on the platform (operating system) you are using.

* [Windows](https://www.google.com/search?q=Windows+install+git)
* [Linux](https://www.google.com/search?q=linux+install+git)
* [Mac](https://www.google.com/search?q=Mac+install+git)

## Authorization fails during git-push command

You need to provide correct username and password. Remember, you are not using your email as username.

# Development

This package is made and tested on CentOS8, but git commands are rather universal. Developers are encouraged to make system-based changes when necessary.

* All the script files should be named starting with 'git-' for compatibility.
* All git-* scripts should include option '--README' as a special case option for generating the README

# Command reference
## git-author
```
git-author "Firstname Lastname" "firstname.lastname@example.com"
```
## git-commit
Automatically adds and commits all files in the repository.
```
git-commit "Commit message here"
```
## git-push
Push commands using branch and origin names
```
git-push master
git-push master origin
```
