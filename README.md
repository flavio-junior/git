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
**Listar o histórico de commits do repositório**
```
git log
```
**Listar todas as branch do projeto**
```
git branch
```
**Adicionar um arquivo**
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
**Fazendo commit de forma direta sem uso do add .**
```
git commit -am "fazendo commit de forma direta"
```
**Para adicionar alterações do projeto sem ter a necessidade de criar um novo commit**
```
git commit --amend --no-edit index.html
```
**Desfazer ação sem defazer as alterações que foram feitas no código**
```
git reset index.html
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
**Exibir os dados que foram adicionados em determinado arquivo**
```
git diff
git diff --staged
git diff --cached
```

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
8. 

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
