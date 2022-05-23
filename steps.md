# Steps
## Now we are going to setup an empty repository in `Github` and setup a `local` repository with only one file, `README.md`
### In Github:
1- Create and empty repository in github and get the link (git@github.com:jcabdi/git_learn.git)
### In local machine:
<<<<<<< HEAD
=======

|Purpose | Command|
--- | ---|
|1-Create project folder and cd into it|`mkdir <project_folder> && cd <project_folder>`
|2-Create README.md and add header|`touch README.md && echo "# Title" >> README.md`|
|3-Initialize git project|`git init` (It creates a .git folder and initialize the local repo)
|4-Include all the files to the next step (commit)|`git add --all` or `git add .`
|5-Commit the "actual" status of the repo|`git commit -m "message describing the commit"`
|6-Add a remote named origin for the repo at the url|`git remote add origin git@github.com:jcabdi/git_learn.git`
|7-Force the actual branch to be called "main"|`git branch -M main`
|8-Updates remote refs origin with local "main"|`git push -v -u origin main`

>>>>>>> a4ca84156cb4db1ee976749faf68295c87dc55af
1-Create project folder and cd into it:
```bash
mkdir <project_folder> && cd <project_folder>
```
2-Create README.md and add main header:
```bash
touch README.md && echo "# Title" >> README.md
```
3-Initialize git project. It creates a .git folder and initialize the local repo:
```bash
git init
```
4-Include all the files to the next step (commit):
```bash
git add --all
```
or
```bash
git add .
 ```
5-Commit the "actual" status of the repo:
```bash
git commit -m "message describing the commit"
```
6-Add a remote named origin for the repo at the url:
```bash
git remote add origin git@github.com:jcabdi/git_learn.git
```
7-Force the actual branch to be called "main":
```bash
git branch -M main
```
8-Updates remote refs origin with local "main":
```bash
git push -v -u origin main
```
<<<<<<< HEAD
=======

>>>>>>> a4ca84156cb4db1ee976749faf68295c87dc55af
