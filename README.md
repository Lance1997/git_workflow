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
- "feature-<'id or description'>" branch which is going to be used to add new features
- make necessary feature changes, commit changes and run command "git checkout dev" to move to the dev branch and run command "git merge feature-<'id or description'>
- run command "git branch -d feature-<'id or description'>" to remove branch after successfully merging unless it might be needed again
