# git_workflow
A sample repo to mimic a proper git workflow

## Start with two branches
- Master Branch and Development Branches
- Master Branch will only store production ready code
- Development Branch will store development codes till its ready to be merged in the master branch

## Process
- Create a repo on github
- Clone repo to local computer
- run command "git checkout -b dev" to create a dev branch
- run command "git push -u origin dev" to create and switch branch for pushing commits("git push") to the dev branch

## Create supporting branches
- Create support branches for new features, releases
- "feature-<id or description>" branch which is going to be used to add new features
- use release branch if you have versions of the software that is going to be committed to allow tracking by release or version of the software
- make necessary feature changes, commit changes and run command "git checkout dev" to move to the dev branch and run command "git merge feature- <id or description>
- run command "git branch -d feature-<id or description>" to remove branch after successfully merging unless it might be needed again
- After successful changes merge develop or dev branch into the master branch for production

## Making Hot fixes
Hotfix is the scenario where a bug needs to be fixed in the master branch as soon as possible and one cannot use the dev branch because changes has already been made to it that is not in production.

- Create a hotfix branch from the master branch with name "hotfix-<id or description>
- Make changes to hotfix branch and merge to master and to the develop branch to allow fix to be in the develop branch too
- You can then delete the hotfix branch if successful with hotfix.
