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


`Removendo uma branch local`

> git branch -d nomeBranch

`Removendo uma branch remota`

> git push origin :nomeBranch


#### Clonando um repositório

> git clone url_do_repositorio


#### Comandos básicos para commits
`Puxando alterações da branch remota/atualizando branch local`

> git pull origin nomeBranch


`Visualizando alterações na branch`

> git status


`Visualizando diferença na alteração de um arquivo`

> git diff nomeArquivo


`Adicionando todos os arquivos alterados/adicionados/removidos ao commit de uma vez`

> git add -A


`Adicionando arquivos ao commit de forma unitária`

> git add nomeDoArquivo


`Gerando o commit`

> git commit -m "Descrição do commit"


`Adicionando arquivos e gerando o commit ao mesmo tempo`

> git commit -am "Descrição do commit"


`Sincronizando commit no github/bitbucket etc.`

> git push -u origin nomeBranch

#### Reescrevendo o último commit

> git commit -m "Mensagem do commit" --amend

#### Removendo todas as alterações de um arquivo

`Antes de dar um git add`
> git checkout nomeArquivo

#### Removendo um arquivo do stage

`Depois de dar um git add`
> git reset -- nomeArquivo

#### Voltando versão do código.
`Voltando para uma versão especifica e ignorando todos os commits à frente`

> git reset --hard codVersao

`Voltando para uma versão especifica e mantendo as modificações dos commits posteriores prontas para um novo commit`
> git reset --soft codVersao

`Voltando para uma versão especifica e mantendo as modificações dos commits posteriores prontas para um novo git add nos arquivos`
> git reset --mixed codVersao

`Revertendo commit sem perder o código e a informação nos logs`
> git revert --no-edit codeCommit

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
