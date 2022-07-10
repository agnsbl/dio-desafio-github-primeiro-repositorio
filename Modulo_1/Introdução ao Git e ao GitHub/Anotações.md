# Introdução ao Git e ao GitHub

Git é um sistema de versionamento (cria versões do trabalho/programa) de código distribuído, criar e monitorar diferentes versões do nosso código. Já o GitHub é onde guarda esse software que cuida do versionamento do código, ou seja, é um repositório online onde é salvo o código.

Alguns benefícios de aprender essas tecnologias está no controle de versão, armazenamento em nuvem, trabalho em equipe (colaboração), melhorar seu código e reconhecimento através da plataforma.





# Navegação via Linha de Comando

A maioria dos sistemas operacionais possuem programas que têm uma interface gráfica (responsiva e interativa), ou seja, um GUI (*graphic user interface*). Já o Git é uma CLI (*command line interface*), forma de interação por meio de linha de comando.

Comandos básicos como: mudar de pastas, listar as pastas, criar e deletar pastas/arquivos. Para usar a linha de comando pelo Windows o seu terminal tem os seguintes comandos: cd, dir, mkdir, del / rmdir. Já no Unix os comandos são diferentes: cd, ls, mkdir, rm -rf.

 

### _OS COMANDOS_

- *DIR / LS:* listar as pastas do diretório

- *CD (change directory):* depois de escrever o cd precisamos colocar " / ", assim teremos mudado o diretório e depois podemos colocar o "dir" para mostrar as pastas dele. Para sair de uma pasta é só colocar "cd .." indo na pasta anterior.

- *CLS (clear screen) / CLEAR:* limpar o terminal (dá pra usar CTRL + L no Windows)

- _TAB (atalho do teclado):_ para o sistema completar o nome automático

- *MKDIR (make directory):* cria uma nova pasta
- *ECHO:* ele apenas "ecoa" o que é escrito no terminal utilizando também o símbolo " > " (redirecionador de fluxo), o qual pega o output/a saída dessa função echo e vai joga em um arquivo, checando se existe uma pasta/arquivo com o nome escrito

- *DEL:* no Windows ele deleta apenas arquivos da pasta e não a pasta em si

- *RMDIR (remove directory) / RM -RF:* deleta o repositório e os arquivos dele

 

OBS: outro atalho de teclado é usar a setinha para cima do teclado para navegar pelo histórico de comandos utilizados





# Como o Git Funciona por Baixo dos Panos

### _SHA1_

É um algoritmo de encriptação, ou seja, ele pega o arquivo e embaralha de uma forma específica (*Secure Hash Algorithm*). Esses dados encriptados geram conjuntos de caracteres de 40 dígitos e esses conjuntos são únicos e servem como identificação. Isso significa que se temos um arquivo de texto muito grande ele vai gerar um conjunto (uma chave) de 40 caracteres e se mudarmos uma vírgula ele vai gerar outro conjunto de 40 caracteres, e se tirarmos essa vírgula e deixarmos o texto original ele vai retornar aquele mesmo conjunto de 40 caracteres original. **É uma forma curta de representar um arquivo**, é uma forma do Git de garantir que os arquivos sofreram alteração e garantir que aquele arquivo possui exatamente aquele conteúdo.



### _OBJETOS INTERNOS DO GIT_

Esses objetos são:

- _BLOBS:_ é o primeiro objeto que conhecemos e tem o tipo do objeto, o tamanho da string e o conteúdo desse arquivo. A partir do momento que sabemos o que o sha1 faz, o Git vai guardar esses arquivos que o sha1 faz gerando a encriptação dele e o Git armazena metadados nesses objetos (ex.: esse blob contém metadados do Git, que são o tipo do objeto, tamanho da string, tamanho do arquivo, etc).
- _TREES:_ as árvores armazenam blobs, ou seja é uma crescente, com a blob sendo o bloco básico de composição, a tree armazenando e apontando para tipos de blobs diferentes e um outro tipo de estrutura de dados que são os commits. A árvore também contém metadados e aponta para um blob, que por sua vez tem um sha1, e ela também guarda o nome desse arquivo (o blob não guarda o nome do arquivo, só o sha1 - caracteres identificadores dele). A árvore vai ser responsável de montar toda a estrutura de onde estão os arquivos, elas podem apontar para blobs ou para outras árvores, e isso porque os diretórios dentro de um sistema operacional podem conter outros diretórios (assim, árvores são objetos recursivos). Árvores também tem um sha1 desse metadado, e as blobs tem o sha1 do arquivo e as árvores apontam para essas blobs. Assim, se mudar uma coisa no arquivo que essa árvore está apontando, o sha1 da bolha vai mudar e isso vai consequentemente mudar o sha1 da árvore.

- _COMMITS:_ objeto mais importante de todos, é o que vai juntar tudo e dar sentido para a alteração que estamos fazendo, ele aponta para uma árvore, para um parente (último commit realizado antes dele), para o autor e para uma mensagem (autor e mensagem fazem parte dessa ideia de sentido). Esses arquivos representados pelas blobs e as pastas representadas pelas árvores representam uma alteração, e podemos escrever uma mensagem nesse     commit que vai dar significado para esses arquivos dentro dessas pastas. Os commits levam timestamp de quando foram criados, e também possuem sha1     e encriptação. Assim, se alterarmos um dado dentro de uma blob (arquivo) ele vai gerar um sha1 dessa blob, e essa blob tem uma árvore apontando para ela de forma que vai alterar o sha1, e o commit aponta para uma árvore que pode apontar para outra árvore; por isso o Git é tão confiável, quando olhamos o histórico de commits temos a certeza que ninguém mexeu nele, temos uma linha do tempo de quais commits foram realizados, temos a certeza de que aquele commit representa exatamente o que queríamos dizer com o código sem a interferência de outras pessoas.

  

### _SISTEMA DISTRIBUÍDO E SEGURO_

Pelo fato dos commits serem tão difíceis de serem modificados, tanto a versão mais recente (que está na máquina do servidor) quanto as versões das pessoas que estão mantendo esse sistema são versões confiáveis. Assim, se der algum problema no Git vai acontecer algo com essas pessoas, porque as versões disponíveis dele também são muito confiáveis, por isso ele é um sistema seguro e distribuído.

 

 

### _CHAVE SSH E TOKEN_

_CHAVE SSH_

Forma de estabelecer uma comunicação segura e encriptada entre duas máquinas. No caso, vamos nos conectar com o servidor do GitHub e vamos configurar a nossa máquina local como uma máquina confiável para o GitHub estabelecendo essa conexão com duas chaves, uma pública e outra privada (a chave pública colocamos no GitHub e a partir desse momento o GitHub vai reconhecer a assinatura da nossa máquina, com uma conexão prévia estabelecida, assim poderemos já enviar códigos por lá sem nem precisar utilizar senha).



_TOKEN DE ACESSO VIRTUAL_

Segunda forma de autenticação segura do GitHub, processo de digitar seu nickname e senha. Nesse caso gera um token de acesso, guarda em um lugar, e sempre que acessarmos o GitHub usamos nosso nickname e depois colocamos nosso token.







# Iniciando o Git e criando um commit

Primeiros comandos com Git

- Iniciar o GIT (*git init)*

- Iniciar o versionamento *(git add)*

- Criar um commit *(git     commit)*

  

### *Criando um repositório*

Podemos lançar o Git Bash a partir do windows (clicar com o botão direito em "Git Bash here" no arquivo desejado), assim o Bash já é aberto direto no repositório que queremos, eliminando a necessidade de navegar pelas pastas.

Com o *git init* começamos com o Git para iniciar e versionar o nosso código. Notar que quando iniciamos o *git init* ele mostra uma nova pasta nessa que a gente criou chamada ".git", no entanto, quando listamos os conteúdos do livro-receitas essa pasta não aparece. Isso é porque ela é uma pasta oculta e uma pasta gerencial do Git, onde ele versiona os objetos que a gente vai manipular.

Para vermos essa pasta, usamos uma flag específica com o ls chamada **" -a "**. Ela que mostra arquivos ocultos, e ao entrar nessa pasta e dar um "ls" vemos que ela já tem uma estrutura lá dentro, estruturas referentes ao próprio Git

Quando um objeto *commit* é criado ele tem o nome de um autor, por isso se nunca usamos o Git na primeira vez ele vai ser configurado pedindo um username e email (o commit tem um autor atrelado a ele). Para configurar isso rodamos os comandos **git config --global user.email** (email) e **git config -- global user.name** (username). Podemos citar essa configuração global ou apenas para esse repositório.

 



### *Adicionando um arquivo*

Adicionamos um arquivo a essa pasta, de tipo **Markdown**, essa é uma forma mais humana de se escrever o arquivo HTML. O arquivo HTML é o esqueleto, estrutura básica de qualquer página da web. A quantidade de hashtags em Markdown funciona como os "h1" "h2" "h3" (...) no HTML.

Commits são os objetos do Git que dão significados para as alterações, e eles carregam uma mensagem de texto assim como o nome do autor junto nos metadados. Por isso precisamos criar uma mensagem de texto quando usando o *git commit*.







# Passo a Passo no Ciclo de Vida

### *TRACKED E UNTRACKED*

Dentro dos arquivos que são rastreados no git existem 3 categorias

1. _Unmodified:_ arquivo que ainda não foi modificado
2. _Modified:_ é o unmodified que sofreu modificação
3. _Staged:_ conceito chave, onde ficam os arquivos que estão se preparando para fazer parte de outro tipo de agrupamento

Também existem os arquivos "Untracked" que são os arquivos que o Git não tem ciência sobre.

Quando usamos o **git add** estávamos com um arquivo untracked porque tínhamos acabado de criar ele, então o Git ainda não sabia da existência dele. Ai quando rodamos o git add ele moveu esse arquivo untracked direto para staged, para a área em que ele está esperando alguma coisa.

No unmodified temos um arquivo dentro do repositório do Git que ainda não sofreu alterações. Se alterarmos algo nele ele vai ser movido para modified automaticamente, isso porque o Git vai comparar o SH1 dos arquivos vendo que os arquivos tem modificações. Se rodar de novo git add nesse arquivo unmodified ele vai para staged, ou seja, também vai para essa área especial que está aguardando alteração. Se existe um arquivo unmodified e esse arquivo é removido, ele vai para untracked porque o Git ainda não tem ciência dele (ele não tinha sofrido alteração nenhuma e ainda foi removido).

Quando movemos nossos arquivos para o staged, onde eles estão esperando fazer alguma coisa, na verdade esses arquivos estão se preparando para fazer parte de um commit! Um commit é um objeto chave do Git. O commit carrega um autor, frase, uma data, e assim que eles integram o objeto commit eles deixam de ser staged e vão para commit. E o commit retorna esses arquivos para unmodified para começar o ciclo de novo, ele pega todos esses arquivos e como termina as alterações deles ele cria um **snapshot** do código naquele momento que está salvo dentro do commit (desse objeto especial). Esses arquivos voltam para o unmodified aguardando novas modificações. Isso é um ciclo entre esses três estágios rastreados.



Quando rodamos o **git init** iniciamos um repositório, e temos dois ambientes:

1. _Servidor:_ sua versão no servidor que é o GitHub
2. _Ambiente de desenvolvimento:_ a versão do Git que está na nossa máquina (tudo que está nela)

Assim, as alterações que fazemos no código na nossa máquina não repercutem imediatamente na versão que está no nosso repositório remoto (remote repository).

No nosso ambiente de desenvolvimento temos o repositório de trabalho, a área de staging e os arquivos vão mudar entre essas áreas. Quando fazemos um commit esses arquivos passam a integrar o repositório local, que por sua vez podem fazer parte de um repositório remoto.

Quando adicionamos um arquivo que era untracked e damos um git add ele é movido para staged. Quando temos um arquivo modificado e damos git add ele também vai para staged (os arquivos vão ficar transitando entre o working directory para a staging area). Quando fazemos o commit fazemos duas coisas: movemos os arquivos que estavam na staging area (tiramos eles daí para unmodified), ou seja, criamos um snapchat dos arquivos naquele momento, e populamos nosso repositório local. O repositório local só vai ser composto por commits, caso não estiver commitado não será possível enviar para um repositório remoto.



O **git status** vai ajudar a monitorar os estados dos arquivos (untracked, unmodified, modified, staged). Para mover arquivos usamos " **mv** " e o " **./** " significa que ele vai desse repositório que a gente está para outro



### _RESUMO_

Quando rodamos o git add estamos movendo os arquivos para staged (sejam eles unmodified ou modified) -> Quando usamos o git commit pegamos todos esses arquivos que estavam em staged, envelopamos eles em uma mensagem (dando significância) e criamos esse objeto chamado commit -> Assim, no diretório de trabalho rodamos o git add, e movemos todos esses arquivos para staged (que vão compor a staging area), e quando usamos o git commit -m passando uma mensagem, movemos essa área de staging para o nosso repositório local.







# Trabalhando com GitHub

É bom usar o mesmo email e nickname cadastrado nos commits que aqueles usados no GitHub. Para recadastrar eles é só usar o seguinte comando  **" git config --global --unset user.name / user.email"**. Depois que usar esse comando fazer um **" git config --list "** para ver se foi descadastrado e depois é só recadastrar com o certo.

Para mover o seu repositório local para um repositório remoto (para uma origem remota) precisamos primeiro adicionar a origem na qual estamos enviando esses arquivos, e para isso utilizamos o **" git remote add origin (colar o link que o GitHub nos dá ao criar um novo repositório) "**. Em seguida, usar o **git remote -v** o qual lista as listas de repositório remotos que temos cadastradas. Esse "origin" é apenas um apelido, é para que não precisamos digitar o endereço https a todo momento, mas por convenção usamos origin.

Ao fazer o git status nos certificamos que não tem nenhuma pendência no repositório. O comando para levar o código do nosso repositório local para o nosso repositório remoto é o **" git push origin master "** , sendo origin o apelido do link que nos demos, e master é a branch que estamos enviando esse código.