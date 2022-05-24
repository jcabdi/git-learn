# Branches

Branches in `git` is a powerful concept, instead of keep working on the main branch (which we could think of as the branch having the final product),
we may add or change contents using branches. When we make a new branch we are putting in the new created branch the actual content of main in the
moment we created this new branch. Now we can add or modify content and all the changes are going to be taking place inside the new branch and main
remain the same.
## Create a new branch and switch to it

```bash
git branch <new-branch-name>
git switch <new-branch-name>
```
or
```bash
git checkout -b <new-branch-name>
```
## List branches
```bash
git branch
```
You will see an asterisk `*` next to the currently checked out branch.
## Switch between branches once created
```bash
git switch <branch-name>
```
or
```bash
git checkout <branch-name>
```
