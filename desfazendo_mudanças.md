# Desfazendo Mudanças

## Para desfazer modificações de arquivos ainda não comittados você pode usar o restore

* **git restore 2_stage_area.md**

## Caso eu tenha adicionado algum arquivo a stage area por engano posso usar o restore --staged para desfazer

* **git restore --staged .DS_Store**
* ou **git restore --staged .** para remover tudo

## Para corrigir o último commit você pode usar o git commit --amend -m "nova mensagem"

* **git commit --amend -m "nova mensagem"**
* só usar em casos de erro ao inserir a mensagem

## Para recuperar um arquivo de um git anterior você pode usar o checkout

* **git checkout 7e87ds -- README.md**
* é importante adicionar um ponto na historia sempre que algo for alterado, pois facilita a recuperação

## Para remover arquivos não rastreados do seu working directory você pode utilizar o git clean

* **git clean -n** para ver o que o comando vai fazer
* **git clean -f** para forçar a remover os arquivos **permanentemente**

## Como reverter mutiplos arquivos, voltar a um ponto da historia e criar um novo commit com o git revert.

* o primeiro passo é o working tree limpo
* **git revert HEAD~5** 
* vai trazer os arquivos desse commit especifico
* você também pode usar o **git log --oneline** e copiar o hash espeficico 
* **git revert 7sfds**

## Ignorando arquivos que não precisam estar dentro dos meus pontos de historia com o .gitignore

* Você pode criar um arquivo de texto com o nome de .gitignore e adicionar o diretorio dos arquivos a serem ignorados dentro do .gitignore
* Arquivo **.gitignore**
* Dentro do arquivo 
* **linha 1 node_module/**
* **linha 2 .DS_Store**
* Caso o arquivo que você queira ignorar já esteja sendo rastreado, você pode remover o rastreamento de todos os arquivos com o comando **git rm -r --cached .** e readicionar todos arquivos com o **git add .** quando você for commitar a alteração, observe que o diretorio inserido dentro do **.gitignore** será ignorado
