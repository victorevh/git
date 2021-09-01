# Criando um repositorio por linha de comando


**echo "# landing-page"** >> README.md
**git init**
**git add README.md**
**git commit -m ":tada: first commit"** commit com icone 
**git branch -M main**
**git remote add origin git@github.com:victorevh/landing-page.git**
**git push -u origin main**

# Caso exista um repositorio existente

**git remote add origin git@github.com:victorevh/landing-page.git**
**git remote -V** para ver os repositorios
**git branch -M main** para mudar a branch de master para main
**git push -u origin main** adicionando o repositorio para upstream

# Puxando alterações feitas na nuvem para repositorio local

**git log --oneline** para verificar os commits
**git pull** traz as modificações online.

# Caso eu altere algum arquivo em outra maquina e esqueça de fazer um **git pull**

* Para resolver o conflito de merge basta
* **git config --global pull.rebase false**
* **git pull**

* Você pode abrir o arquivo em conflito, onde vai mostrar a sua HEAD atual e você pode editar ou não o que você quer.
* ou você pode abrir o arquivo no Visual Code Studio e aceitar ou recusar as alterações locais.
* após as alterações basta fazer o **git pull** o **git push** e commitar as alterações
