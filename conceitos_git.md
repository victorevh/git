# Conceitos Git

## Fluxo padrão

#

#### Para iniciarmos utilizamos o git init

* **git init**

#### Para puxarmos outro projeto utilizamos o git clone

* **git clone**

#### Feito isso o git inicia um repositorio local, os arquivos que estão nesse repositorio estão na etapa do Working Diretory

#### Para preparar o arquivo para ser commitado (Stage Area) utilizamos o git add

* **git add**

#### Feito isso o arquivo já está preparado para ser commitado, e assim podemos utilizar o git commit para jogar os arquivos para o Local Repository

* **git commit -m " "**

#### É nesse momento que o arquivo é adicionado ao ponto na historia.

#

## Git Worflow

* Working Diretory (file.txt (v1)) > git add > 
* Stage Area (file.txt(v1)) > git commit -m "primeira linha do tempo" >
* Local Repository (file.txt(v1)) primeira linha do tempo
#
* Working Diretory (file.txt (v2)) > git add > 
* Stage Area (file.txt(v2)) > git commit -m "segunda linha do tempo" >
* Local Repository (file.txt(v2)) segunda linha do tempo / primeira linha do tempo
#
* Working Diretory (file.txt (v3)) > git add > 
* Stage Area (file.txt(v3)) > git commit -m "terceira linha do tempo" >
* Local Repository (file.txt(v3)) terceira linha do tempo / segunda linha do tempo / primeira linha do tempo

#
## Hash Values (SHA-1)

* checksum - converte dados em numeros


#### parent: null
#### author: Victor Oliveira        ======== 9f5fdf5d40c =========> Snapshot A
#### message: Initial Commit
#
#### parent: 9f5fdf5d40c
#### author: Victor Oliveira        ======== 4f48asdf8aw =========> Snapshot B
#### message: Second Commit
#
#### parent: 4f48asdf8aw
#### author: Victor Oliveira        ======== 6sbd32948fs =========> Snapshot C
#### message: Thrid Commit

#
## HEAD

* É um ponteiro que demonstra qual ponto da historia estamos.

**Master** é a linha linha do tempo, o **HEAD** aponta sempre qual parte da linha do tempo *master* você está

#### Você pode visualizar o diretorio disponivel dentro da pasta invisivel do git com o comando **cat .git/HEAD**

* Ao visualizar o diretorio de HEAD, você pode obter o numero do commit utilizando o comando **cat .git/refs/heads/master**

* Você pode utilizar o comando **git status** para verificar o status atual do seu git

* Para remover algum arquivo da **Stage Area** você pode utilizar o comando **git rm --cached file1.txt** 