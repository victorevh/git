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
