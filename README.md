# projetoGit
Projeto  Git 
PASSO A PASSO:
 
NO GITHUB

CRIAR CONTA; 

DEPOIS, VAI EM NEW PARA CRIAR NOVO REPOSITÓRIO;

ADICIONE O NOME E TAMBÉM UMA DESCRIÇÃO (OPCIONAL);

DEIXAR PÚBLICO OU PRIVADO;

FAZ A MARCAÇÃO DO READ.MS FILE;

AS DEMAIS MARCAÇÕES DEIXAR EM BRANCO;

CLICA NO BOTÃO 'CREATE REPOSITORY';


NO GIT BASH 

VAMOS SEGUIR A SEQUENCIA QUE SEGUE, NESTE CASO EU TIVE ALGUNS CONFLITOS E DEIXEI PARA QUE POSSAM VER, PORÉM, CASO NÃO TENHAM, É SÓ SEGUIR PARA O PRÓXIMO COMANDO.

AQUI ESTAÇAO A LEGENDA DOS COMANDOS EM ORDEM NO GIT:
GIT CLONE (url do projeto copiado do github) 
CD (nomedoseuprojetonasuamaquina)
CODE .
LS
GIT STATUS
GIT ADD .
GIT STATUS
GIT COMMIT -M "(mensagem/arquivos/etiqueta)"
GIT CHECKOUT -B ...(novabranch)...
GIT PUSH ORIGIN ...(novabranch)...




SEGUE AS SEQUENCIAS DE COMANDOS E O DESCRITIVO DOS RETORNOS PARAR IDENTIFICAÇÃO:

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio
$ git clone https://github.com/ElendeBona/projetoGit.git
Cloning into 'projetoGit'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio
$ cd projetoGit

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ code .

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ ls
README.md  index.html  index.js

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        index.js

nothing added to commit but untracked files present (use "git add" to track)

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git add .

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html
        new file:   index.js


edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git commit -m "Primeiros arquivos"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'edsoo@Bona.(none)')

ADENDO_CONF USERNAME AND EMAIL 

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git config --global user.email "edsoolbj@gmail.com"

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git config --local user.name "ElendeBona"

edsoo@Bona MINGW64 /c/ESTUDO/Portfolio/projetoGit (main)
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=edsoolbj@gmail.com
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=https://github.com/ElendeBona/projetoGit.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
branch.main.remote=origin
branch.main.merge=refs/heads/main
user.name=ElendeBona

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git reflog

ADENDO_DOCODIGOMAIN

be5cd01 (HEAD -> main) HEAD@{0}: commit: arquivos iniciais
7eaa3b2 (origin/main, origin/HEAD) HEAD@{1}: clone: from https://github.com/ElendeBona/projetoGit.git

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git checkout -b novos-arquivos-git
Switched to a new branch 'novos-arquivos-git'

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (novos-arquivos-git)
$ git push origin novos-arquivos-git

ADENDO_AQUI ABRIU O GITHUB PARA AUTENTICAÇÃO E SÓ APARECEU ESTA MENSAGEM ABAIXO QUANTO O PROCESSO LÁ FOI CONCLUÍDO

Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'novos-arquivos-git' on GitHub by visiting:
remote:      https://github.com/ElendeBona/projetoGit/pull/new/novos-arquivosgit
remote:
To https://github.com/ElendeBona/projetoGit.git
 * [new branch]      novos-arquivos-git -> novos-arquivos-git


DE VOLTA AO GITHUB

SEGUIR A SEQUENCIA:
VAI MOSTRAR UM BOTÃO DESTACADO DE COMPARE & PULL REQUEST, QUE MOSTRA TODAS AS ALTERAÇÕES QUE FORAM FEITAS NA MAQUINA NO VSCODE E PRECISAM APARECER TAMBÉM AQUI NO REPOSITORIO GIT (LOCAL) E DO GITHUB (SERVIDOR), CONFORME A FIGURA


OBSERVAÇÃO: COMO FOI FEITO MAIS DE UMA TENTATIVA E ESTA É VERSÃO QUE PELO VISTO ESTÁ FUNCIONANDO, PORTANTO, TORNARÁ OFICIAL, O ARQUIVO LOCAL NA MÁQUINA FOI CRIADO NA ÁREA DE TRABALHO DIFERENTE DO CAMINHO PENSADO ANTERIORMENTE. PORTANTO, MAIS PRA FRENTE PRECISAREI MUDAR O LOCAL DE ORIGEM E NOVAMENTE SINCRONIZAR COM O GITHUB.
 
NA SEQUENCIA, VAI PEDIR SE QUER DAR UM MERGE E É EXATAMENTE QUE PRECISAMOS FAZER, PORQUE IREMOS MISTURAR E SINCRONIZAR OS DOIS, O REPOSITORIO LOCAL (MAQUINA) COM REPOSITORIO WEB/SERVIDOR (GITHUB) - IREI DAR UM MERGE - QUE SIGNIFICA FAZER A MISTURA, UNIÃO ENTRE OS ARQUIVOS QUE ESTÃO NA MÁQUINA E SUAS ATUALIZAÇÕES (UPDATES) COM O QUE JÁ EXISTE DE ARQUIVOS NO GITHUB.
 
 
RESUMO 
 
PARA CONSEGUIR REALMENTE FINALIZAR COM SUCESSO TODO O PROCESSO EU TIVE QUE ASSISTIR 3 VÍDEOS NO YOUTUBE, QUE SÃO:

Camis Monteiro - passo a passo explicativo para criar repositório no github, enviando seus arquivos SEM ERROS
https://www.youtube.com/watch?v=XHzuovv2vMQ
 
ERRO CONFIGURE USERNAME AND EMAIL -
JavaTCoding - Solved: Git please tell me who you are error | How to Configure Username & Email using Git Bash
https://www.youtube.com/watch?v=dRNcbhx2698


E TAMBÉM DA RAFAELLA BALLERINI - QUE NÃO CONSEGUI FAZER O PROCESSO DA DA FORMA COMO ELA FEZ, MAS ME AUXILIOU PARA ENTENDER A AUTENTICAÇÃO (QUE SEMPRE PEDEM QUANDO É PRIMEIRA VEZ PRA TUDO, PRA BAIXAR VSCODE, CRIAR CONTA GITHUB, CRIAR REPOSITÓRIO, BAIXAR O GIT (BASH - ADM, ETC) E ALGUNS OUTROS CONCEITOS E COMANDOS.
Rafaella Ballerini - COMO USAR GIT E GITHUB NA PRÁTICA! - desde o primeiro commit até o pull request! 2/2
https://www.youtube.com/watch?v=UBAX-13g8OM&t=602s


REFIZ O PROCESSO TODO NO GIT SEM ERROS, PORTANTO, PODE SEGUIR POR ESTE OU PELO QUE TROUXE ACIMA

edsoo@Bona MINGW64 ~/OneDrive/Desktop
$ git clone ^[[200~https://github.com/ElendeBona/projetoGit.git~
Cloning into 'projetoGit.git~'...
fatal: protocol '?[200~https' is not supported

edsoo@Bona MINGW64 ~/OneDrive/Desktop
$ git clone https://github.com/ElendeBona/projetoGit.git
Cloning into 'projetoGit'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.


edsoo@Bona MINGW64 ~/OneDrive/Desktop
$ cd projetoGit

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ code .

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ ls
 README.md            index.html
'git passo a passo'   index.js

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        git passo a passo
        index.html
        index.js

nothing added to commit but untracked files present (use "git add" to track)

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git add .

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   git passo a passo
        new file:   index.html
        new file:   index.js


edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git commit -m " arquivos iniciais  "
[main be5cd01]  arquivos iniciais
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 git passo a passo
 create mode 100644 index.html
 create mode 100644 index.js

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git reflog
be5cd01 (HEAD -> main) HEAD@{0}: commit: arquivos iniciais
7eaa3b2 (origin/main, origin/HEAD) HEAD@{1}: clone: from https://github.com/ElendeBona/projetoGit.git

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (main)
$ git checkout -b novos-arquivos-git
Switched to a new branch 'novos-arquivos-git'

edsoo@Bona MINGW64 ~/OneDrive/Desktop/projetoGit (novos-arquivos-git)
$ git push origin novos-arquivos-git
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'novos-arquivos-git' on GitHub by visiting:
remote:      https://github.com/ElendeBona/projetoGit/pull/new/novos-arquivosgit
remote:
To https://github.com/ElendeBona/projetoGit.git
 * [new branch]      novos-arquivos-git -> novos-arquivos-git
 