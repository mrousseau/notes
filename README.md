# notes

## VS Code Extensions
```
- akamud.vscode-theme-onedark
- druideinformatique.antidote
- emilast.LogFileHighlighter
- GitHub.vscode-pull-request-github
- midnightsyntax.vscode-wrap-console-log
- ms-azuretools.vscode-docker
- MS-CEINTL.vscode-language-pack-fr
- ms-dotnettools.csharp
- ms-kubernetes-tools.vscode-kubernetes-tools
- ms-mssql.data-workspace-vscode
- ms-mssql.mssql
- ms-mssql.sql-bindings-vscode
- ms-mssql.sql-database-projects-vscode
- ms-ossdata.vscode-postgresql
- ms-vscode-remote.remote-containers
- ms-vscode-remote.remote-wsl
- ms-vscode.powershell
- redhat.vscode-yaml
- rodrigovallades.es7-react-js-snippets
```


## script
````
#!/bin/bash

# Mise à jour des packages
sudo apt update

# Installation des dépendances
sudo apt install -y software-properties-common apt-transport-https wget

# Importation de la clé GPG Microsoft
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg

# Ajout du référentiel VSCode
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

# Installation de VSCode
sudo apt update
sudo apt install -y code

echo "Visual Studio Code a été installé avec succès!"

code --install-extension akamud.vscode-theme-onedark --force
code --install-extension druideinformatique.antidote --force
code --install-extension emilast.LogFileHighlighter --force
code --install-extension GitHub.vscode-pull-request-github --force
code --install-extension midnightsyntax.vscode-wrap-console-log --force
code --install-extension ms-azuretools.vscode-docker --force
code --install-extension MS-CEINTL.vscode-language-pack-fr --force
code --install-extension ms-dotnettools.csharp --force
code --install-extension ms-kubernetes-tools.vscode-kubernetes-tools --force
code --install-extension ms-mssql.data-workspace-vscode --force
code --install-extension ms-mssql.mssql --force
code --install-extension ms-mssql.sql-bindings-vscode --force
code --install-extension ms-mssql.sql-database-projects-vscode --force
code --install-extension ms-ossdata.vscode-postgresql --force
code --install-extension ms-vscode-remote.remote-containers --force
code --install-extension ms-vscode-remote.remote-wsl --force
code --install-extension ms-vscode.powershell --force
code --install-extension redhat.vscode-yaml --force
code --install-extension rodrigovallades.es7-react-js-snippets --force

echo "Fin d'installation des extensions"

````
