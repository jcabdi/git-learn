# Setup steps
## Now we are going to setup an empty repository in `GitHub` and setup a `local` repository with only one file, `README.md`
### In GitHub
1- Create and empty repository in GitHub and get the link just created which is pointing to the new repository (git@GitHub.com:`username`/`repo-name`.git)
### In your local machine
1-Create project folder and cd into it
```bash
mkdir <project_folder> && cd <project_folder>
```
2-Create README.md and add main header
```bash
touch README.md && echo "# Title" >> README.md
```
3-Initialize git project. It creates a .git folder and initialize the local repository
```bash
git init
```
4-Include all the files for the next step. This step is `staging` the files you want to include to get them ready to be `commited`
```bash
git add --all
```
or
```bash
git add .
 ```
5-Commit the "actual" status of the repository:
```bash
git commit -m "message describing the commit"
```
6-Add a remote named origin for the repository at the url:
```bash
git remote add origin git@GitHub.com:`username`/`repo-name`.git
```
7-Force the actual branch to be called "main":
```bash
git branch -M main
```
8-Updates remote refs origin with local "main":
```bash
git push -v -u origin main
```

