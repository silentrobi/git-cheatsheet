## Git Rebase
Suppost master branch is ahead of your feature branch commits. Therefore to align with master branch and get rid of much more conflicts rebase is useful.
So, what you do is get latest commits from master and add your branch commits on top of it. 

`git rebase master`

[**More detail**](https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase#:~:text=What%20is%20git%20rebase%3F,of%20a%20feature%20branching%20workflow.)

**Two types of rebasing**:

- Git Rebase Standard 
- Git Rebase Interactive

>**Interactive rebasing** is useful when you by mistake did hard reset and you want to add those commits back to working history.
But for that 

# Reduce your commits to one commit

1. Check your new commits from `git log`. Suppose new commits count is 5.
2. Do soft reset that keeps changes. `git reset HEAD~5 --soft`
3. Now add all the changes. `git add .`
4. Commit changes to single commit. `git commit -m "single commit"`



# Git commands

- check changes: `git status`
- init git to project: `git init`
- create branch: `git checkout -b branchA`
- switch to branch: `git checkout branchA`
- commit with message
