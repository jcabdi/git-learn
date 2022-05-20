### In Github:

1- Create and empty repository in github and get the link (git@github.com:jcabdi/git_learn.git)

In local machine:

|Purpose | Command|
--- | ---|
|1-Create project folder and cd into it|mkdir project_folder && cd project_folder
|2-Create README.md and add header|touch README.md && echo "# Title" >> README.md|
|3-Initialize git project|git init (It creates a .git folder and initialize the local repo)
|4-Include all the files to the next step (commit)|git add --all or git add .
|5-Commit the "actual" status of the repo|git commit -m "message"
|6-Add a remote named origin for the repo at the url|git remote add origin git@github.com:jcabdi/git_learn.git
|7-Force the actual branch to be called "main"|git branch -M main
|8-Updates remote refs origin with local "main"|git push -v -u origin main

