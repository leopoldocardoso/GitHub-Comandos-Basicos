# Comandos básicos do git

1 - inicializando o repositório git:

    git init

2 - clonando repositório do git para máquina local:

    git clone < url do repositório >

3 - adcionando arquivo ao repositorio git:

    git add . ==> adiciona todos os arquivos

    git add < nome do arquivo > ==> adciona apenas o arquivo 

4 - salvando (comitando) alteração de vários arquivos em um só comando:

     git commit -a -m < "mensagem do commit" >

5 - enviando o arquivo paro repositório remoto:

				    git push origin main 

6 - removendo arquivo do git:
    
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