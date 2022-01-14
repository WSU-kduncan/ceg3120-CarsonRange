# Git Guide

## Commands
- clone - Uses ssh to download a copy of the repo to your local system

`git clone git@github.com:Redhawk18/baritone.git`

- add - addes a file(s) to be tracked by github

`git add main.java`

- rm - removes a file

`git rm object.java`

- commit - stages like a checkpoint to be pushed later to the main repo it **should** have a describive message about what the changes are

`git commit -m "describive message"`

- push - checks github for updates, incase github is more updated than your local system, and then sends your staged commits to github as the newest changes

`git push`

- fetch - is the command to see the new commit history instead of going to github and looking at it

`git fetch`

- merge - this is used to send branches that went well back into the master/main branch since the feature is stable

```
git checkout master
git merge test
```

- pull - this syncs your local system's files with what is on the repo, only helpful if you have friends helping you program.

`git pull`

- branch - prints your current branch with a star, and other common branchs you've been on

- checkout - switches you between branches

`git checkout map-art-builder`

## Git files & folders
- .git folder - to keep it simple, the .git folder holds all the github info you have and need for the repo

- .gitingore - this is the file where you tell git not to upload junk or sercets, things like built files, libary junk, and tokens.

## GitHub
- pull requests - you fixed someone elses code, or made them a completely new feature and out of the goodness of your heart you want everyone to gain from this change, so the owner or someone with permission can pull your changes into the repo

- SSH authentication - used since passwords can easily be compromised, and keys are much safer since they are unique

