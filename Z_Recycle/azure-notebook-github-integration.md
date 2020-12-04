# Integrating Azure Jupyter notebooks with github  
See https://medium.com/@mikeclymer/integrating-azure-notebooks-jupyter-notebooks-with-github-fd847e941e4  
See also
* https://notebooks.azure.com/help/libraries/creating/import-from-github  
* https://git-scm.com/book/en/v2   
  * https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup  
  * https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration  

## Overview
1. Create [github](https://github.com/) repository
2. Import to [Azure notebooks](https://notebooks.azure.com)
3. Use the [Azure terminal](https://notebooks.azure.com/help/libraries/terminal) to configure git
4. Sync files between Azure & github using `push` & `pull`
5. Use `status` to see what has been modified & needs to be `commit`ed


### Git Configuration 
Set your local Git configuration for access to your remote GitHub repository.
```PowerShell
cd ~/library  
ls -l
git config --global user.name "roguetrainer"  
git config --global user.email ian.r.c.buckley@gmail.com 
git config push.default simple
git config -l  
```
Sample output:
```
nbuser@nbserver:~/library$ git config -l
user.email=ian.r.c.buckley@gmail.com
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
remote.origin.url=https://github.com/roguetrainer/systemic-risk
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
branch.master.remote=origin
branch.master.merge=refs/heads/master
push.default=simple
```
### Push
```PowerShell
git push
``` 
Sample session:
```
nbuser@nbserver:~/library$ git push
Username for 'https://github.com': roguetrainer
Password for 'https://roguetrainer@github.com': <ENTER-PASSWORD>
Everything up-to-date
nbuser@nbserver:~/library$ ^C
nbuser@nbserver:~/library$
```

### `git` + `add`, `commit`, `push`, `log`
From Mike Clymer's blog:
* See what is untracked using `status`
* `add` the new (e.g. notebook)  
* `commit`
* `push`
* `log`
```PowerShell
git status
git add newnotebook.ipynb
git commit -am "Adding somenotebook.ipynb"
git push
git log
```
Sample session:
```
nbuser@nbserver:~/library$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   azure-notebook-github-integration.md

no changes added to commit (use "git add" and/or "git commit -a")
nbuser@nbserver:~/library$ git commit -a
[master 040a506] Small corrections
 1 file changed, 15 insertions(+), 1 deletion(-)
```
## `git pull`
```
git pull
```

If things get modified at both ends, try:
```
git reset --hard origin/master
```
