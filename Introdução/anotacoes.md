# Comando básicos para um bom desempenho no terminal :pencil2:

* dir: informa os diretórios que existem dentro da pasta, ou seja, ele lista todas as pastas. No linux utiliza o ls;

* cd /: leva para a base do diretório c do windows;

* cd: utilizado para acessar uma pasta, ou seja, entrar em uma pasta;

* cd .. : retrocede uma pasta, ou seja, quando vc deseja sair da pasta;

* cls: limpa o terminal;
 
* mkdir: cria uma pasta;

* echo hello > hello.txt: irá criar um arquivo dentro da pasta, sendo que dentro do arquivo irá jogar a informação do echo que foi hello;

* del: deletar arquivos e repositórios. Note que ele não removeu a pasta teste, porém ele deletou o arquivo hello.txt que havia no interior dele. 

* rmdir teste /S /Q : irá apagar a pasta teste junto com o seu arquivo. Nesse caso, a pasta é deletada.
 
# Entendendo como o Git funciona por debaixo dos panos :pencil2:

* A sigle "SHA" significa que o git aplica criptografia em seu arquivo. A saída dessa encriptação gera um conjunto de caracteres identificador de 40 dígitos. Esse conjunto de caracteres é único e serve para identificação. Assim, o git utiliza essa criptação para identificar e acessar os arquivos de forma rápida. Importante frisar que o git não utiliza apenas para identificação dos arquivos, mas também para os objetos que existem no próprio git.
  
* Os objetos internos do Git são BLOBS, TREES e COMMITS que irão versionar o nosso código. Os arquivos ficam armazenados no BLOB onde se encontram os metadados. Isso quer dizer que o git ao criptar o arquivo ele adiciona metadados, sendo esses ficam salvos no objeto Blob.   

* O outro objeto é a TREE que são objetos que irão armazenar os BLOBS, ou seja, ela armazena e aponta para blobs diferentes. Ela também contém metadados. Veja que a árvore aponta para um BLOB que tem SHA1 que possui um arquivo. Além disso, as árvores podem apontar para outras árvores diferentes. Cada árvore também tem um SHA1.  
  
* O COMMIT é outro objeto que irá juntar tudo. Aqui cada COMMIT também terá um SHA1. Um COMMIT aponta para uma árvore. Se alterar um arquivo, o seu BLOB será alterado, sendo que os metadados da TREE e do COMMIT também serão alterados. 




