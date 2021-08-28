# O que é o GIT?

* Sistema de controle de versão distribuido
* Open-source
* Pontos na história: commit (viagem no tempo)
    * Histórico de alterações no código
    * Voltar para qualquer ponto na história
* Controlar o fluxo de novas funcionalidades
    * Ramificações: branch (universos paralelos)
    * Vários devs no mesmo projeto
    * Análise e resolução de conflitos

## Configuração inicial

* Essa configuração você fará apenas uma vez por computador e o efeito se manterá após atualizações.

* Você também pode muda-las em qualquer momento rodando esses comandos novamente.

## Sua identidade

####  Assim que instalar o git, abra o terminal e digite

* $ git config --global usar.name "Seu Nome Completo Aqui Entre Aspas"
* $ git config --global user.email seuemailaaqui@dominio.com.br

#### Isso é importante porque cada commit usa esta informação, e ela é carimbada de forma imutável nos commits que você começa a criar:

* Se você quiser substituir essa informação com nome diferente para um projeto específico, você pode rodar o comando sem a opção --global dentro daquele projeto

## Editor

#### Você poderá trocar o editor padrão, que é o VIM, por outro, para isso basta:

* git config --global core.editor "code -w"

## Ver configurações

#### Você poderá verificar suas configurações com o comando abaixo

* git config --list

# Git Config

* Permite ver e atribuir variáveis de configuração como nome e email
* Estas variáveis podem ser armazenadas em três lugares diferentes:
    * 1. /etc/gitconfig : válido para todos os usuários no sistema e todos os seus repositórios. Se você passar a opção --system para git config, ele lê e escreve nesse arquivo.
    * 2. ~/.gitconfig ou ~/.config/git/config : Somente para o seu usuário. Você pode fazer o Git ler e escrever neste arquivo passando a opção --global .
    * 3. config no diretório Git (ou seja, .git/config ) de qualquer repositório que você esteja usando: especifico para esse repositorio.

* Cada nível sobreescreve os valores no nível anterior, ou seja, valores em .git/config prevalecem sobre /etc/gitconfig.

## SSH Keys

* Para obter SSH key vc deve utilizar o comando
**ssh-keygen -t rsa -b 4096 -C "victor_oliveirasantos@hotmail.com"**
* Para visualizar o title e a key você pode acessar o diretorio
**cd .ssh/.id_rsa.pub** e ver o arquivo com o **cat id_rsa.pub**
* Copie o arquivo do **id_rsa.pub** e colar no git hub
* Após isso você deve inserir o comando **eval `ssh-agent -s`** 
* em seguita utilize o comando **ssh-add ~/.ssh/id_rsa** para adicionar a identidade

#### No Windows, o arquivo .gitconfig estará no diretório $HOME que é C:/Users/$USER

* Você pode criar um diretorio com o mkdir, e depois iniciar o diretorio com o comando git init 
* Você pode acessar o diretorio .git com o comando cd e verificar o diretorio com comando ls - a
* Você pode ver as configurações do diretorio com o cat config
* Você pode utilizar o comando pwd para ver em qual diretorio você está

### Para verificar os comandos disponiveis pelo git, basta utilizar o comando git help , caso você deseje ser mais especifico, pode usar o comando diretamente para o conceito, ex: git help log

## Iniciando repositorio git

* Para iniciar um repositorio git, navegue até o diretorio desejado e digite o comando git init

* Para verificar o diretorio você pode utilizar o comando ls -a

* Para verificar todo seu historicos de ações utilize o comando ls -al .git , vale lembrar que caso você apague a pasta invisivel do .git, você perde todo o historico.

## O primeiro Commit


