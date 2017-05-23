# Development Guide

## Work Flow

1. On GitHub, create new issue
2. Create new branch based on the master one, with branch name is the same as the issue title
3. On local, do the following commands to checkout the new branch
```
git checkout master
git fetch
git checkout new-branch-name
```
4. Start the development
5. Do the following commands to push changes to remote
```
git add .
git cz
git push
```
6. After pushing, go to working GitHub repository, view the working branch, then click Pull Request
7. Done
8. Repeat the step 1 for another issues

Notes:
- On Step 1, make sure the title as short as possible and provide issue's description if needed.
- On Step 5, while `git za`, make sure to select the type of changes correctly. If it's a new feature, select `feat`. If it's a bug fix, select `fix`, etc.
- On Step 5, while `git cz`, also don't forget to mention the issue id in the comment (Step 2 of `git cz`). For example `Close #21`. Should use the following verbs to refer to an issue `close, closes, closed, fix, fixes, fixed, resolve, resolve, resolved`. GitHub will automatically close the issue when it's Pull Request is merged to master.