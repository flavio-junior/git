<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain-wordmark.svg" />
  
# ***Tipos de sistemas de controle de versão***
* Local Version Control Systems ```Sistemas de controle de versão local```
* Centralized Version Control Systems ```Sistema de controle de versão centralizado```
* Distributed Version Control Systems ```Sistema de controle de versão distribuido ```

# ***Os três estados principais do git***
* Modified - Alterações feitas nos arquivos que ainda não foram confirmadas no banco de dados.
* Staged - O arquivo modificado foi selecionado e as alterações feitas no projeto deve ser salvas na próxima versão do projeto. 
* Committed - Versão do projeto, armazenada com segurança em um banco de dados local.

# ***Ajuda***

***Geral***
```
git help
```

***Comandos específicos***
```
git help add
git help commit
git help status
```

***Atualizações rápidas de ajuda utilizando o -h***
```
git add -h
```

# ***Alterar configurações do sistema*** 
***Ver a versão do git instalada na máquina***
```
git --version
```
***Verificar as configurações do usuário na máquina que foi instalado o git***
```
git config -l
git config --list
```
***Visualizar todas as suas configurações e aonde estão sendo utilizadas***
```
git config --list --show-origin
```

***Adicionar nome do usuário em nivel global***
```
git config --global user.name "Flávio Júnior"
```
***Adicionar e-mail do usuário em nivel global***
```
git config --global user.email flaviojunior.work@gmail.com
```
***Adicionar nome da branch em nivel global***
```
git config --global init.dafaultBranch master
```

# ***Criando repositório local***
***Iniciar repositório***
```
git init
```
***Verificar status do repositório***
```
git status
git status -s 
git status --short
```
***Abrir o projeto no Visual Studio Code***
```
code .
```
# ***Adicionar um arquivo ou diretório na staging area***
***Adicionar um arquivo***
```
git add arquivo.txt
```
***Adicionar todos os arquivos criados recentemente***
```
git add .
```
***Visualizar as mudanças aplicadas em arquivos que foram modificados mesmo depois que foram enviados para staging area***
```
git diff
```
***Visualizar as mudanças aplicadas em determinado arquivo***
```
git diff --staged
git diff --cached
```
***Remover arquivo***
```
git reset index.html
```
***Desfazer ação***
```
git restore index.html
```
***Desfazer add***
```
git restore --staged contato.html
```
# ***Commit*** 
***Commit simples***
```
git commit
```
***Realizar commit com os arquivos modificados e enviados para  a área de planejamento***
```
git commit -m "Implementando recursos na página principal do site"
```
***Commit de parâmetro único***
```
git commit -am "Commit de parâmetro único"
```
***Para adicionar alterações do projeto sem ter a necessidade de criar um novo commit***
```
git commit --amend
git commit --amend --no-edit
```
***Defazer uma ação indesejada dentro do projeto***
```
git checkout -f 
```
***Listar o histórico de commits do repositório***
```
git log
git log --oneline
```
***Listar o histórico de commits do repositório em uma única linha***
```
git log --oneline
```
***Listar o último commit do repositório***
```
git log -1 HEAD
```
***Desfazer commit sem apagar os arquivos modificados no projeto***
```
git reset 0d27528ebba6650b0a70d59d529983b81adf2962 
```
***Desfazer alterações e voltar para um commit especifico***
```
git reset --hard 3e39bbcd5d0e62aa612bb848ccb5fea77f07ffbc
```
***Desfazer o último commit sem desfazer as alterações realizadas no ultimo commit no repositório local***
```
git reset --soft HEAD~1
```
***Excluir último commit salvo no repositório remoto***
```
git push -f origin master
```
***Listar uma quantidade de commits especificos para excluir***
```
git rebase -i HEAD~4
```
***Resultado do comando anterior***
```
pick 5e3670f Implementando recursos na página principal do site
pick c0abaf2 Página de contato
pick 9dc5ab1 Página sobre
pick a652e8a Página home

# Rebase 5611ed4..a652e8a onto 5611ed4 (4 commands)
#
# Commands:
# p, pick <commit> = use commit
# r, reword <commit> = use commit, but edit the commit message
# e, edit <commit> = use commit, but stop for amending
# s, squash <commit> = use commit, but meld into previous commit
# f, fixup [-C | -c] <commit> = like "squash" but keep only the previous
#                    commit's log message, unless -C is used, in which case
#                    keep only this commit's message; -c is same as -C but
#                    opens the editor
# x, exec <command> = run command (the rest of the line) using shell
# b, break = stop here (continue rebase later with 'git rebase --continue')
# d, drop <commit> = remove commit
# l, label <label> = label current HEAD with a name
# t, reset <label> = reset HEAD to a label
# m, merge [-C <commit> | -c <commit>] <label> [# <oneline>]
# .       create a merge commit using the original merge commit's
# .       message (or the oneline, if no original merge commit was
# .       specified); use -c <commit> to reword the commit message
#
# These lines can be re-ordered; they are executed from top to bottom.
#
# If you remove a line here THAT COMMIT WILL BE LOST.
#
# However, if you remove everything, the rebase will be aborted.
#
```
***Excluindo commit especifico***
```
pick 5e3670f Implementando recursos na página principal do site
pick c0abaf2 Página de contato
drop 9dc5ab1 Página sobre
pick a652e8a Página home
```
***Excluir um arquivo ou diretóro***
```
git rm index.html
```
***Renomear arquivo***
````
git mv index.html contato.html
````


# ***gitignore***
***Nomeação de um arquivo gitignore***
```
.gitignore
```
***Ignorar um arquivo especifico***
``` 
arquivos_secretos.txt 
``` 
***Ignorar tipos de arquivos especificos***
```
*.txt
```

# ***Repositório Remoto***
***Clonar repositório remoto***
```
git clone https://gist.github.com/2545add34e4fec21ec16.git
```
***Clonar repositório com SSH***
```
git remote set-url repository git@github.com:flavio-junior/git.git
```
***Exibir informações do repositório remoto***
```
git remote show origin
```
***Listar todos os repositórios remotos contidos no repositório local***
```
git remote
git remote -v
```
***Vincular repositório local ao repositório remoto***
```
git remote add origin https://github.com/flavio-junior/git-crash.git
```
***Salvar modificações do repositório local no repositório remoto***
```
git push origin main 
git push -u origin main
```
***Baixar modificações salvas no repositório remoto para o repositório local***
```
git pull
```
***Baixar uma branch especifica***
```
git pull origin master
```
***Renomeando repositório remoto***
```
git remote rename origin repository 
```
## ***Tags***
***Criando uma tag simples***
```
git tag v1.0
```
***Tag anotada***
```
git tag -a v2.0 -m " "
```
***Listar todas as tags do repositório***
```
git tag
git tag -l
```
***Exibir informações de um arquivo especifico***
```
git show v1.0
```
***Excluir uma tag***
```
git tag -d v1.0
```
***Criar uma tag através de um commit especifico***
```
git tag v1.0 5611ed4
```
***Salvar uma tag criada no repositório local para o repositório remoto***
```
git push origin v1.0
```
***Salvar várias tags criadas no repositório local para o repositório remoto***
```
git push --tags
```
## ***Git Aliases***
***Definindo apelidos para instruções especificas***
```
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
```

## ***Branches***
***Criar uma branch***
```
git branch testing
git switch -c adones
```
***Listar todas as branch do projeto***
```
git branch
git branch -l
```
***Alterar o nome da branch***
```
git branch -m "main"
```
***Excluir uma branch***
```
git branch -d secondary
```
***Navegar até uma branch especifica***
```
git checkout master
git switch testing
```
***Voltar para a branch anterior***
```
git switch -
```
***Criar uma branch alternativa***
```
git checkout -b secondary
```
***Juntar branch secundária com a principal***
```
git merge secondary
```
***Abortar merge***
```
git merge --abort
```
***Adicionar branch do repositório remoto no repositório local***
```
git pull origin master
```

# ***Rebase***
```

```

# CMD
Comandos básicos para usar no terminal:
1. mkdir - criar uma pasta
2. dir - exibi todos os arquivos listados em um diretório especifico
3. cls - limpa todos os comandos digitados no pront de comando
4. cd - acessa determinada pasta através da rota especificada pelo usuário
6. cd.. - voltar 
7. ipconfig - Para verificar o ip da máquina

  Siglas  | Definição |
:---------|:----------|
 Branches | Galho da árvore
 CVS | Sistema de controle de versão
 Untracked | Não creckeado
 Unmodified | Não modificado
 Modified | Modificado
 Staged | Área de planejamento
 Untracked files | arquivos não crackeado
 Changes to be committed | Alterações confirmadas
 Staging area | Area de planejamento
 Lightweight | Referência para um certo commit salva em um arquivo dentro da pasta .git
 Annotaded | Objeto salvo no banco de dados  que contém informações sobre quem criou, uma mensagem e podem ser assinadas e verificadas GNU Privacy Guard.
 Aliases | Apelido
 Merge | Mesclar
 Rebase | 
**Referências:**
[Git - Documentation](https://git-scm.com/doc)
