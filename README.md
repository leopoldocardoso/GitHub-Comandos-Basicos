## Comandos básicos do git utilizando GitHub ##

### O objetivo deste readme é facilitar o uso do github no dia a dia de estudantes e profissionais de TI que façam utilização desta poderosa ferramnenta de versionamento

1 - Inicializando o repositório git

    git init

2 - Clonando repositório do git para máquina local

    git clone < url do repositório >

3 - Adcionando arquivo ao repositorio git

    git add . ==> adiciona todos os arquivos

    git add < nome do arquivo > ==> adciona apenas o arquivo

4 - Salvando (comitando) alteração de vários arquivos em um só comando

     git commit -a -m < "mensagem do commit" >

5 - Enviando o arquivo paro repositório remoto

    git push origin main

6 - Removendo arquivo do git

    git rm < nome do arquivo >

5 - Verificando os logs

    git log

6 - Movendo ou renomeando arquivos no git

    git mv < nome do arquivo aquivo do nome> ==> renomeia o arquivo

    git mv diretório/arquivo1 diretório-02/arquivo1 ==> move o arquivo entre diretórios

7 - Atualiza repositório local com os dados do respositório remoto

    git pull

8 - Desfazendo alterações no arquivo

    git checkout < nome do arquivo >

9 - Resetando a branch mesmo após commit

    git reset --hard origin/main ==> resetando a branch main

10 - Criando branch

    git branch < nome da branch >

11 - Deletando branch

    git branch -d < nome da branch >

12 - Mudando de Branch

    git checkout <nome da branch>

13 - Criando branch e mudando para branch criada

    git checkout -b <nome da nova branch>

14 - Unindo branch (merge entre branchs)

    git merge <nome da branch>

15 - Desfazendo e salvando alterações no código (funciona apenas em arquivos não comitados)

    git stash

    Obs: O stash funciona como uma lixeira do git. Ao realizar uma alteração no código posso digitar o comando < git stash > que ele salva a alteração em uma stash e desfaz estas alterações em uma stash atual.

16 - Recuperando stash

    git stash list ==>> lista as stashs criadas

    git apply stash <numero da stash> ==> restaura a stash

17 - Removendo stashs

    git stash clear ==> remove todas as stashs

    git stash drop <número da stash> ==> remove apenas a stash específica

18 - Criação de tag

    git tag -a <versão da tag> -m <"mensagem de commit">

    Obs: as tags são úteis para salvar um ponto do código

19 - Visualização da tag

    git show tag <nome da tag>

20 - Navegando entre tags

    git tag checkout <nome da tag>

21 - Enviando tag para o repositório

    git push origin <nome da tag>

22 - Enviando tag para o repositório

    git push origin <nome da tag>

23 - Encontrando branchs remotas

    git fetch -a

24 - Utilizando o remote

    git remote -v ==> visualizaos repositórios no git

    git remote add origin <link do repositorio> ==> adciona um repositório remoto

    git remote rm origin ==> remove o repositório remoto

25 - Adicionando submódulos

    Antes dos comandos, uma breve descrição do que é submódulos:
    - Submódulo é a maneira que temos de possuir dois ou mais projetos em um só repositório;
    - Podemos adicionar uma dependência ao nosso projeto atual, porém mantendo em estruturas separadas.

    git submodule add <repositório> ==> adiciona uma submódulo

    git submodule ==> verifica os submódulos

26 - Git Show: Apresenta informações úteis de um branch.

    git show < nome da branch >

27 - Exibindo diferenças entre branchs

     git diff < nome da branch >

28 - Git shortlog: Este comando apresenta um log de forma resumida do projeto e o nome dos usuários que realizaram alterações

    git shortlog