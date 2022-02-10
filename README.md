# CMD
Comandos básicos para usar no terminal:
1. mkdir - criar uma pasta
2. dir - exibi todos os arquivos listados em um diretório especifico
3. cls - limpa todos os comandos digitados no pront de comando
4. cd - acessa determinada pasta através da rota especificada pelo usuário
6. cd.. - voltar 
7. ipconfig - Para verificar o ip da máquina
8. 


# Git 

Siglas:
* Untracked - Arquivo não rastrado ou crackeado
* Unmodified - Não modificado
* Modified - Modificado
* Staged - Area de planejamento
* Commit - Responsável pelo histórico de versão do repositório. Salva, registra, cria e altera arquivos, registrados em determinado periodo de tempo

Comandos básicos para o usar no terminal com o git:
1. git init - Inicia um repositório git.
2. git status - Verifica e informa o status dos arquivos listados no repositório.
3. git status -s - Flag ou indicado informado para imprimir arquivos no formato curto.
4. git status --short - indicado informado para imprimir arquivos no formato curto.
5. git add . - Adiciona todos os arquivos que estão na pasta.
6. git add README.md - Para adicionar apenas um arquivo especifico.
7. git reset index.html - Para resertar uma arquivo especifico.
8. git diff - Mostra as mudanças que foram feita em determinado arquivo.
9. git diff --staged - Mostra as mudanças que foram feita em determinado arquivo.
10. git diff --cached -- sinonimo de git diff --staged.
11. git commit - Cria um commit.
12. git restore - desfazer uma ação em determinado arquivo.
13. git log - Histórico.
14. git commit -m "Esse é um commit em uma única linha" - commit em uma única linha.
15. git restore --staged - desfazer add .
16. rm - deletar arquivo.
17. git commit -am "descrição do commit" - fazendo commit de forma direta.
18. git mv index.html contato.html - Renomeia um arquivo especifico.
19. git commit --amend --no-edit - Para adicionar alterações no projeto sem ter a necessidade de criar um novo commit e adicionando a último commit.
20. git reset 5545fa56dfc94501d3a120ea22ea7876c6c191d8 - Desfazer o último commit para um commit especifico de acordo com o commit que foi informado pelo usuário porém não desfaz as alterações no projeto.
21.  git reset --hard 5545fa56dfc94501d3a120ea22ea7876c6c191d8 - Dezfazer o úlitimo commit completo sem deixar arquivos do commit que foi desfeito.
22.  git rebase -i HEAd~2 - Para excluir um commit especifico.
23.  git checkout -f - Defazer uma ação indesejada dentro do projeto.
24.  git remote -v Listar todos os servidores remotos dentro do projeto.
25.  git branch - Lista todas as branchs do projeto.
26.  git push origin master - Para subir o repositório local para a branch master.
27.  git clone - Clonar determinado projeto.


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
 
 
 
 
 

