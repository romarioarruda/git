### Reforçando conhecimentos de git

`Iniciando um repositório`

> git init

#### Configurações adicionais básicas

`Configurando username`

> git config --global user.name "usuario"

`Configurando email`

> git config --global user.email "email do usuario"

`Vendo todas as configurações`

> git config --list

`Criando nova branch`

> git branch nomeBranch

`Mudando para outra branch`

> git checkout nomeBranch

`Visualizando branch atual`

> git branch

`Removendo uma branch`

> git branch -d nomeBranch

`Visualizando alterações na branch`

> git status

`Adicionando todos os arquivos alterados/adicionados/removidos ao commit`

> git add -A

`Adicionando arquivos ao commit de forma unitária`

> git add nomeDoArquivo

`Gerando o commit`

> git commit -m "Descrição do commit"

`Adicionando arquivos e gerando o commit ao mesmo tempo`

> git commit -am "Descrição do commit"

`Sincronizando commit no github`

> git push origin nomeBranch

`Voltando para uma versão especifica e ignorando todos os outros a frente`

> git reset --hard codVersao

`Voltando para uma versão especifica e mantendo as modificações dos commits posteriores prontas para um novo commit`
> git reset --soft codVersao

`Voltando para uma versão especifica e mantendo as modificações dos commits posteriores sem o git add`
> git reset --mixed codVersao
