#Git Commands

## Setup
### Creating an SSH Key
This allows your computer to access github without repeatedly typing your password.

	ssh-keygen -t rsa -b 4096
	cd .ssh
	
get public key from this directory, use this to authorise github to access your computer:

	cat id_rsa.pub
	
### Setting your Username & Email Address for connecting to Github
	git config --global user.email "example@email.com"
	git config --global user.name "usernamehere"

## Creating a Repository
	git init # initialise a repository

**Stage and commit at this point (see below) then create the online repository on github. Don't let github put any files in it, then push the repository to GitHub:**

	git remote add origin URL # add the local git repository to a remote git server (IE github)
	git push -u origin master # -u means set upstream, sets the default upstream for pushing, origin is a friendly name for the location I push to, master is the name of the branch I push to

## Getting Remote Content
	git clone URL # clone a remote repository to my computer
	git pull # pull changes from the remote git server

## Using your git repository
	git add * # add all files in the repo
	git stage * # add/remove/change all in prep for committing
	git rm # remove a file
	git ignore FILEPATH # adds a file to .gitignore, creates .gitignore if necessary

	git commit -m "this is a comment" # commit with a comment
	git push
	git status
	git diff FILEPATH # see changes since last commit

	git checkout # Grabs the latest version of a file from the repository and adds it to local copy, overwriting existing

## Submodules
	git submodule add URL
	git submodule update # pull the submodules in the repo, needed for updating submodules, & for when repo is cloned to another computer

