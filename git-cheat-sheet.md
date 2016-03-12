Git Commands

create ssh key:
ssh-keygen -t rsa -b 4096
cd .ssh
get public key from this directory, use this to authorise github to access your computer


git init # initialise a repository

git remote add origin URL # add the local git repository to a remote git server (IE github)

git push -u origin master # -u means set upstream, sets the default upstream for pushing, origin is a friendly name for the location I push to, master is the name of the branch I push to

git clone URL # clone a remote repository to my computer
git add * # add all files in the repo
git stage * # add/remove/change all in prep for committing
git rm # remove a file
git ignore FILEPATH # adds a file to .gitignore, creates .gitignore if necessary

git commit -m "this is a comment" # commit with a comment
git push
git pull
git status
git diff FILEPATH # see changes since last commit
git submodule add URL
git submodule update # pull the submodules in the repo, needed for updating submodules, & for when repo is cloned to another computer

