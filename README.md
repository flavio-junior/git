## Tipos de sistemas de controle de versão
* Local Version Control Systems ```Sistemas de controle de versão local```
* Centralized Version Control Systems ```Sistema de controle de versão centralizado```
* Distributed Version Control Systems ```Sistema de controle de versão distribuido ```

## Os três estados principais do git
* Modified - Alterações feitas nos arquivos que ainda não foram confirmadas no banco de dados.
* Staged - O arquivo modificado foi selecionado e as alterações feitas no projeto deve ser salvas na próxima versão do projeto. 
* Committed - Versão do projeto, armazenada com segurança em um banco de dados local.

## Ajuda

**Geral**
```
git help
```

**Comandos específicos**
```
git help add
git help commit
git help status
```

**Atualizações rápidas de ajuda utilizando o -h**
```
git add -h
```

## Checando configurações 
**Verificar as configurações do usuário na máquina que foi instalado o git**
```
git config -l
git config --list
```
**Visualizar todas as suas configurações e aonde elas estão sendo utilizadas**
```
git config --list --show-origin
```

**Adicionar nome do usuário em nivel global**
```
git config --global user.name "Flávio Júnior"
```
**Adicionar e-mail do usuário em nivel global**
```
git config --global user.email flaviojunior.work@gmail.com
```
**Adicionar nome da branch em nivel global**
```
git config --global init.dafaultBranch master
```

## Inicializando um repositório em um diretório existente
**No windows**
```
C:\Users\Info\Documents\git\git-repository>
```
**Iniciar repositório**
```
git init
```
**Verificar status do repositório**
```
git status
git status -s 
git status --short
```
**Abrir o projeto no Visual Studio Code**
```
C:\Users\Info\Documents\git\git-repository>code .
```
**Listar o histórico de commits do repositório**
```
git log
```
**Listar todas as branch do projeto**
```
git branch
```
**Exibir as mudanças adicionados ou removidas em determinado arquivo**
```
git diff
git diff --cached
```
## Adicionar um arquivo ou diretório na **staging area**
**Adicionar um arquivo**
```
git add arquivo.txt
```
**Adicionar todos os arquivos criados recentemente**
```
git add .
```
**Visualizar as mudanças aplicadas em arquivos que foram modificados mesmo depois que foram enviados para staging area**
```
git diff
```
**Visualizar as mudanças aplicadas em determinado arquivo**
```
git diff --staged
```
**Remover arquivo**
```
git reset index.html
```
**Desfazer add**
```
git restore --staged contato.html
```
## Fazer commit 
**Commit**
```
git commit
```
**Commit de parâmetro único**
```
git commit -am "Commit de parâmetro único"
```
**Fazendo commit de forma direta sem uso do add .**
```
git commit -am "fazendo commit de forma direta"
```
**Para adicionar alterações do projeto sem ter a necessidade de criar um novo commit**
```
git commit --amend --no-edit index.html
```
**Desfazer ação**
```
git restore index.html
```
**Defazer uma ação indesejada dentro do projeto**
```
git checkout -f 
```
**Desfazer alterações e voltar para um commit especifico**
```
git reset --hard 3e39bbcd5d0e62aa612bb848ccb5fea77f07ffbc
```
**Excluir arquivo ou diretóro**
```
git rm index.html
```
**Renomear arquivo** 
````
git mv index.html contato.html
````

24. git remote -v Listar todos os servidores remotos dentro do projeto.
26. git push origin master - Para subir o repositório local para a branch master.
27. git clone - Clonar determinado projeto.

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
 Branches | Galho
 CVS | Sistema de controle de versão
 Untracked files | arquivos não crackeado
 Changes to be committed | Alterações confirmadas
 Staging area | Area de planejamento
 -n, --dry-run         | dry run
 -v, --verbose         | be verbose
 -i, --interactive     | interactive picking
 -p, --patch           | select hunks interactively
 -e, --edit            | edit current diff and apply
 -f, --force           | allow adding otherwise ignored files
 -u, --update          | update tracked files
 --renormalize         | renormalize EOL of tracked files (implies -u)
 -N, --intent-to-add   | record only the fact that the path will be added later
 -A, --all             | add changes from all tracked and untracked files
 --ignore-removal      | ignore paths removed in the working tree (same as --no-all)
 --refresh             | don't add, only refresh the index
 --ignore-errors       | just skip files which cannot be added because of errors
 --ignore-missing      | check if - even missing - files are ignored in dry run
 --chmod (+|-)x        | override the executable bit of the listed files
 --pathspec-from-file <file> | read pathspec from file
 --pathspec-file-nul   | with --pathspec-from-file, pathspec elements are separated with NUL character

# Observações
para ignorar determinado arquivo ou arquivos em um repositório é necessário criar o seguinte arquivo dentro do seu projeto:

 ``` .gitignore ```
 
 Para ignorar um arquivo no seu repositório é só colocar o nome do arquivo dentro do .gitignore:
 
 ``` arquivos_secretos.txt ```
 
 Para ignorar arquivos especificos:
 
 ``` *.txt ```
 
 ## Repositório Remoto
 Clonar repositório
 
 CLONE - clonar repositório
 
 FETCH - é utilizado para baixar as referência do projeto principal que está hospedado no servidor
 
 PUSH - Subir o histórico de versionamento para o servidor 
 
 PULL
 
**Referências:**

[Git - Documentation](https://git-scm.com/doc)
