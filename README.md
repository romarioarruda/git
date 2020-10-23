### Reforçando conhecimentos de git

`Iniciando um repositório`

> git init

#### Configurações iniciais básicas

`Configurando username`

> git config --global user.name "usuario"

`Configurando email`

> git config --global user.email "email do usuario"

`Vendo todas as configurações`

> git config --list

#### Branchs

`Criando nova branch`

> git branch nomeBranch


`Mudando para outra branch`

> git checkout nomeBranch


`Visualizando branch atual`

> git branch


`Removendo uma branch`

> git branch -d nomeBranch

#### Removendo todas as alterações de um arquivo

`Antes de dar um git add`
> git checkout nomeArquivo

#### Comandos básicos para commits
`Visualizando alterações na branch`

> git status


`Visualizando diferença na alteração de um arquivo`

> git diff nomeArquivo


`Adicionando todos os arquivos alterados/adicionados/removidos ao commit`

> git add -A


`Adicionando arquivos ao commit de forma unitária`

> git add nomeDoArquivo


`Gerando o commit`

> git commit -m "Descrição do commit"


`Adicionando arquivos e gerando o commit ao mesmo tempo`

> git commit -am "Descrição do commit"


`Sincronizando commit no github`

> git push -u origin nomeBranch


#### Voltando versão do código.
`Voltando para uma versão especifica e ignorando todos os commits à frente`

> git reset --hard codVersao

`Voltando para uma versão especifica e mantendo as modificações dos commits posteriores prontas para um novo commit`
> git reset --soft codVersao

`Voltando para uma versão especifica e mantendo as modificações dos commits posteriores sem o git add dos arquivos`
> git reset --mixed codVersao
>

#### Mesclando duas branchs

`Juntando alterações entre duas branchs usando o git merge`
> git checkout nomeBranch `Precisamos estar dentro da branch que queremos mesclar com a master`
>
> git merge master `fazendo o merge entre a branch especifica e a master`
>
`Juntando alterações entre duas branchs usando o git rebase`
> git checkout nomeBranch `Precisamos estar dentro da branch que queremos mesclar com a master`
>
> git rebase master `fazendo o rebase entre a branch especifica e a master`
>

Entenda melhor sobre `git merge` e `git rebase` neste post: [link](https://www.treinaweb.com.br/blog/git-merge-e-git-rebase-quando-usa-los/)


#### Revertendo commit sem perder o código (Salvador de sexta feira)

`Commit que será desfeito sem perder a informação nos logs`
> git revert --no-edit codeCommit
