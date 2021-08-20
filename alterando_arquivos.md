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
* * Para verificar quais palavras exatamente foram modificadas, você também pode utilizar o --color-words
* **git show 83d7c84e3401 --color-words**

## Como deletar arquivos no git com o remove

* **git rm file1.txt**  
* Após remover o arquivo, você deve commitar a alteração 
* Ao remover o arquivo diretamente pelo git, você pula a etapa de adicionar o arquivo deletado para a stage área.

## Como renomear arquivos no git com o move

* **git mv repository_local.md 1-repository_local.md**
* Após renomear o arquivo você deve commitar a alteração
* Ao renomear o arquivo diretamente pelo git, você pula a etapa de adicionar o arquivo deletado para a stage área 

## Movendo arquivos no git com o move

* **git mv README.md sub/README.md**
* Após mover o arquivo você deve commitar a alteração 
* Ao mover o arquivo diretamente pelo git, você pula a etapa de adicionar o arquivo para a stage area.
