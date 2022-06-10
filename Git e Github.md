# Introdução ao Git e GitHub



Comandos básicos do terminal Windows:

* mkdir = criar um diretório

* echo = criar um arquivo

* cd = navegar entre as pastas do sistema

* cd .. = voltar uma pasta

* dir = listar pastas

* ls -a = listar pastas ocultas (.git)

* mv = mover

* CTRL + L = limpar o terminal

* del = deletar apenas arquivos

* rmdir /s /q = deletar diretórios

  

  ## Funcionamento do GIT

  * SHA1 (Secure Hash Algorithm): Algoritmo de encriptação que gera um conjunto único de caracteres com 40 dígitos dos dados criptografados.

  * Objetos: 

    * BLOBS = Armazena metadados, o tipo, tamanho e conteúdo do arquivo.

    * TREE = Resolve o problema de armazenar o nome de arquivo e também permite armazenar de forma conjunta um grupo de arquivos e também permite armazenar de forma conjunta um grupo de arquivos, apontam para tipo de blobs ou para outras tree.

    * COMMITS = Armazena qualquer tipo de informações em formato binário dando sentido ao conteúdo.

      Apontam para uma ou mais TREE, uma mensagem e um autor.

      O commit é impossível de ser alterado, fazendo com que cada versão do código seja confiável

  ### Primeiros comandos com GIT

  Antes de tudo é necessário estabelecer uma conexão segura e encriptada, pública e privada.

  Realizada a encriptação é necessário criar um autor no git, usando os comandos:

  Git config –global user.email “xxxxxxx@xxxx.xxx”

  Git config – global user.name Xxxx Xxxx.

​		

		* git init = Iniciar
		* git add = adicionar arquivos
		* git commit -m "MENSAGEM" = criar um commit
		* git status = status atual do diretório (untracked, unmodified, modified, staged)
		* git clone + caminho copiado = copiar diretório

#### Enviar o diretório para o servidor remoto

* git remote add origin + LINK 

  O "origin" é apenas um apelido para não digitar o HTTP, por exemplo.

* git push origin master = empurra o diretório para remoto

#### Conflito de Merge



Um possível erro acontece quando há 2 alterações na mesma linha e o github deixa o usuário realizar a alteração.

Neste caso é necessário usar o comando Git pull origin master para puxar o diretório e realizar a alteração.

Após feito, segue o mesmo caminho para o commit (git add * e depois git commit)