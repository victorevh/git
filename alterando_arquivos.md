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

## Verificando os pontos da historia criado

* **git log**

## Como verificar modificações no **working directory** com o git diff

* **git diff**

## Como verificar modificações na **stage area** com o git diff --staged

* **git diff --staged**

## Como deletar arquivos no git com o remove

* **git rm file1.txt**  
* Após remover o arquivo, você deve commitar a alteração 
* Ao remover o arquivo diretamente pelo git, você pula a etapa de enviar o arquivo deletado para a stage área.

## Como renomear arquivos no git com o move

* **git mv repository_local.md 1-repository_local.md**
* Após renomear o arquivo você deve commitar a alteração
* Ao renomear o arquivo diretamente pelo git, você pula a etapa de enviar o arquivo deletado para a stage área 
