# Set global configuration

    git config --global user.name "Qwe Rty"
    git config --global user.email qwe@rty.com



# Initiate repo

    git init --bare __repo__.git
    git clone /path/to/__repo__.git
    git remote add origin /path/to/__repo__.git
    git push origin master



# Run locally

Check remote URLs:

    git remote -v

List branches:

    git branch

Delete branch:

    git branch -d <branch_name>

List changed files:

    git status

Stage all changed files:

    git add --all

Commit all stages:

    git commit -a

Show list of commits:

    git log --oneline
    git log --graph --all --decorate --abbrev-commit



# Take changes from USER

    cd /path/to/ME/__repo__
    git pull /path/to/__USER__/__repo__



# Update remote repo

    cd /path/to/remote/__repo__
    git pull /path/to/ME/__repo__



# Or from local

    git checkout master -f



# Delete commit

    git log
    git reset --hard 6f493481f771ca795e25c029a2054edeaac95e69
    git tag -d V.1.0.0
    cd /path/to/__repo__
    rm -R V.1.0.0
    rm -R default
    ln -s V.0.1.31 default

