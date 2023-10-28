# Comandos básicos do git

1 - inicializando o repositório git

    git init

2 - clonando repositório do git para máquina local

    git clone < url do repositório >

3 - adcionando arquivo ao repositorio git

    git add . ==> adiciona todos os arquivos

    git add < nome do arquivo > ==> adciona apenas o arquivo 

4 - salvando (comitando) alteração de vários arquivos em um só comando

     git commit -a -m < "mensagem do commit" >

5 - enviando o arquivo paro repositório remoto

    git push origin main 

6 - removendo arquivo do git
    
    git rm < nome do arquivo >

5 - verificando os logs

    git log

6 - movendo ou renomeando arquivos no git

    git mv < nome do arquivo aquivo do nome> ==> renomeia o arquivo
    
    git mv diretório/arquivo1 diretório-02/arquivo1 ==> move o arquivo entre diretórios

7 - atualiza repositório local com os dados do respositório remoto

    git pull

8 - desfazendo alterações no arquivo

    git checkout < nome do arquivo >

9 - resetando a branch mesmo após commit

    git reset --hard origin/main ==> resetando a branch main

10 - criando branch

    git branch < nome da branch >

11 - deletando branch

    git branch -d < nome da branch >

12 - mudando de Branch

    git checkout <nome da branch>

13 - criando branch e mudando para branch criada

    git checkout -B <nome da nova branch>

14 - unindo branch (merge entre branchs)

    git merge <nome da branch>

15 - desfazendo e salvando alterações no código (funciona apenas em arquivos não comitados)

    git stash

    Obs: O stash funciona como uma lixeira do git. Ao realizar uma alteração no código posso digitar o comando < git stash > que ele salva a alteração em uma stash e desfaz estas alterações em uma stash atual.

16 - recuperando stash

    git stash list ==>> lista as stashs criadas

    git apply stash <numero da stash> ==> restaura a stash

17 - removendo stashs

    git stash clear ==> remove todas as stashs

    git stash drop <número da stash> ==> remove apenas a stash específica
    