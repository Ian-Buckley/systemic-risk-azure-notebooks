# Integrating Azure Jupyter notebooks with github  
See https://medium.com/@mikeclymer/integrating-azure-notebooks-jupyter-notebooks-with-github-fd847e941e4  
See also
* https://notebooks.azure.com/help/libraries/creating/import-from-github  
* https://git-scm.com/book/en/v2   
  * https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup  
  * https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration  

## Overview
1. Create github repository
2. Import to Azure notebooks
3. Use the Azure terminal to configure git
4. Sync files between Azure & github

## Open Azure terminal
Enter the commands in the Azure terminal in your browser:
https://notebooks.azure.com/help/libraries/terminal 

## Initial set up 
```PowerShell
cd ~/library  
ls -l
```

## Git Configuration 
```PowerShell
git config --global user.name "John Doe"  
git config --global user.email johndoe@example.com  
git config push.default simple
git config -l  
```

## Push
```PowerShell
git push
``` 
