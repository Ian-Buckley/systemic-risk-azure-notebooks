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
4. Sync files between Azure & github


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

