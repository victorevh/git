# Alterando Arquivos

## Criando novos arquivos e editando

* **touch file.txt** para criar um novo arquivo
* **VIM file.txt** para editar o arquivo criado com o VIM

## Adicionando/preparando arquivos para serem commitados com o git add

* **git add file.txt**  adiciona um arquivo especifico
* **git add .** adiciona todos os arquivos da stage area
* **git add * .js** (sem espaço entre o *.js) adiciona todos arquivos de uma determinada extensão

## Verificando status dos arquivoss do working directory/stage area

* **git status**

## Criando commits

* **git commit -m 'first commit'**

## Commitando um arquivo já rastreado

* Quando você modificar um arquivo já rastrado, você pode utilizar o comando -a para passar do working directory e stage area para Repository local
* **git commit -am "modify index"**

## Verificando os pontos da historia criado

* **git log**

## Como verificar modificações no **working directory** com o git diff

* **git diff**

## Como verificar quais palavras exatamente foram modificadas com o git diff --color-words

* **git diff --color-words**

## Como verificar modificações na **stage area** com o git diff --staged

* **git diff --staged**

## Como verificar modificações realizadas de um commit para o outro com o nº do hash

* **git show 83d7c84e3401**
* Para verificar quais palavras exatamente foram modificadas, você também pode utilizar o --color-words
* **git show 83d7c84e3401 --color-words**

## Como verificar modificações realizadas em um arquivo ou pasta especifica de um commit com o nº do hash

**git show aa69518b72b4d226e9 -- src/views/index.hbs** para verificar um arquivo especifico ou você pode usar o * para verificar todos os arquivos do diretorio

## Como deletar arquivos no git com o remove

* **git rm file1.txt**  
* Após remover o arquivo, você deve commitar a alteração 
* Ao remover o arquivo diretamente pelo git, você pula a etapa de adicionar o arquivo deletado para a stage área.

## Como remover o rastreamento de um arquivo com o git remove

* **git rm -r --cached .DS_Store** ou **git rm -r --cached .** para remover o rastreamento de todos os arquivos

## Como renomear arquivos no git com o move

* **git mv repository_local.md 1-repository_local.md**
* Após renomear o arquivo você deve commitar a alteração
* Ao renomear o arquivo diretamente pelo git, você pula a etapa de adicionar o arquivo deletado para a stage área 

## Movendo arquivos no git com o move

* **git mv README.md sub/README.md**
* Após mover o arquivo você deve commitar a alteração 
* Ao mover o arquivo diretamente pelo git, você pula a etapa de adicionar o arquivo para a stage area.

## Ignorando arquivos que não precisam estar dentro dos meus pontos de historia com o .gitignore

* Você pode criar um arquivo de texto com o nome de .gitignore e adicionar o diretorio dos arquivos a serem ignorados dentro do .gitignore
* Arquivo **.gitignore**
* Dentro do arquivo 
* **linha 1 node_module/**
* **linha 2 .DS_Store**
* Caso o arquivo que você queira ignorar já esteja sendo rastreado, você pode remover o rastreamento de todos os arquivos com o comando **git rm -r --cached .** e readicionar todos arquivos com o **git add .** quando você for commitar a alteração, observe que o diretorio inserido dentro do **.gitignore** será ignorado
