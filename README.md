# Guia básico de comandos do git

## Ajuda

**Geral**
```
git help
```

**Comandos específico**
```
git help add
git help commit
git help status
```
## Configurações 

Adicionar nome do usuário em nivel global
```
git config --global user.name "Flávio Júnior"
```
Adicionar e-mail do usuário em nivel global
```
git config --global user.email flaviojunior.work@gmail.com
```
Adicionar nome da branch em nivel global
```
git config --global init.dafaultBranch master
```
# Comandos do git:
**Iniciar repositório**
```
git init
```
**Verificar status do repositório**
```
git status
```
**Listar o histórico de commits do repositório**
```
git log
```
**Listar todas as branch do projeto**
```
git branch
```
**Adicionar um arquivo em específico**
```
git add arquivo.txt
```
**Adicionar todos os arquivos criados recentemente**
```
git add .
```
**Desfazer add**
```
git restore --staged contato.html
```
**Fazer um commit**
```
git commit
```
**Commit de parâmetro único**
```
git commit -am "Commit de parâmetro único"
```
**Fazendo commit de forma direta sem uso do add<arquivo> ou add .**
```
git commit -am "fazendo commit de forma direta"
```
**Desfazer ação sem defazer as alterações que foram feitas no código**
```
git reset index.html
```
**Desfazer ação**
```
git restore index.html
```
Defazer uma ação indesejada dentro do projeto.
```
git checkout -f 
```
**Desfazer ação e voltar para um commit especifico**
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
 
1.  fdf 
2. git status
3. git status -s - Flag ou indicado informado para imprimir arquivos no formato curto.
4. git status --short - indicado informado para imprimir arquivos no formato curto.
5. git add . 
6. git add README.md - Para adicionar apenas um arquivo especifico.
7. git reset index.html -
8. git diff - Mostra as mudanças que foram feita em determinado arquivo.
9. git diff --staged - Mostra as mudanças que foram feita em determinado arquivo.
10. git diff --cached -- sinonimo de git diff --staged.
11. git commit - 
12. git restore - 
13. git log -
14. git commit -m 
15. git restore --staged - 
16. rm - 
17. git commit -am "descrição do commit" - 
18. git mv index.html contato.html - 
19. git commit --amend --no-edit - Para adicionar alterações no projeto sem ter a necessidade de criar um novo commit e adicionando a último commit.
20. git reset 5545fa56dfc94501d3a120ea22ea7876c6c191d8 - Desfazer o último commit para um commit especifico de acordo com o commit que foi informado pelo usuário porém não desfaz as alterações no projeto.
21. git reset --hard 5545fa56dfc94501d3a120ea22ea7876c6c191d8 
22. git rebase -i HEAd~2 - Para excluir um commit especifico.
23. git checkout -f - 
24. git remote -v Listar todos os servidores remotos dentro do projeto.
26. git push origin master - Para subir o repositório local para a branch master.
27. git clone - Clonar determinado projeto.

**Git - Sistema de controle de versão de arquivos**

Siglas:
* Untracked - Arquivo não rastrado ou crackeado
* Unmodified - Não modificado
* Modified - Modificado
* Staged - Area de planejamento
* Commit - Responsável pelo histórico de versão do repositório. Salva, registra, cria e altera arquivos, registrados em determinado periodo de tempo

# CMD
Comandos básicos para usar no terminal:
1. mkdir - criar uma pasta
2. dir - exibi todos os arquivos listados em um diretório especifico
3. cls - limpa todos os comandos digitados no pront de comando
4. cd - acessa determinada pasta através da rota especificada pelo usuário
6. cd.. - voltar 
7. ipconfig - Para verificar o ip da máquina
8. 

# Observações
para ignorar determinado arquivo ou arquivos em um repositório é necessário criar o seguinte arquivo dentro do seu projeto:

 ``` .gitignore ```
 
 Para ignorar um arquivo no seu repositório é só colocar o nome do arquivo dentro do .gitignore:
 
 ``` arquivos_secretos.txt ```
 
 Para ignorar arquivos especificos:
 
 ``` *.txt ```
 
 # Como trabalhar com repositórios remotos?
 **CLONE**
 ```
 
 ```
 **FETCH**
 ```
 
 ```
 **PUSH**
 ```
 
 ```
 **PULL**
 ```
 
 ```
 
 CLONE - clonar repositório
 
 FETCH - é utilizado para baixar as referência do projeto principal que está hospedado no servidor
 
 PUSH - Subir o histórico de versionamento para o servidor 
 
 
**Referências:**

[Git - Documentation](https://git-scm.com/doc)
