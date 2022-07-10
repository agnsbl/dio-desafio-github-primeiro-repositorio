# Pensamento Computacional

### _INTRODUÇÃO AO PENSAMENTO COMPUTACIONAL_

Pensamento computacional é o processo de pensamento envolvido na expressão de soluções em passos computacionais ou algoritmos que podem ser implementados no computador (ou seja, ele não se restringe apenas ao computador). É um pensamento sistemático e eficiente tanto na formulação e resolução de problemas, e tem que ser capaz de resolver tanto por uma máquina tanto por um ser humano.

* _Decomposição:_ dividir um problema complexo em subproblemas

* _Reconhecimento de padrões:_ identificar padrões ou tendências

* _Abstração:_ extrapolar o conceito do problema para uma forma generalista

* _Design de algoritmos:_ automatizar, definir passo a passo da solução do problema



### _HABILIDADES COMPLEMENTARES_

* _Raciocínio lógico:_ uma forma de pensamento estruturado, ou raciocínio, que permite encontrar a conclusão ou determinar a resolução de um problema

* _Aperfeiçoamento:_ objetivo de que a partir de uma solução, determinar pontos de melhora e refinamento



### _DECOMPOSIÇÃO_

Decomposição é o primeiro passo da resolução de problemas dentro do conceito de pensamento computacional. "Dado um problema complexo, devemos quebrar ele em problemas menores. Portanto, problemas mais fáceis e gerenciáveis"

Temos estratégias:

* _Análise:_ processo de quebrar e determinar partes menores e gerenciáveis

* _Síntese:_ combinar os elementos recompondo o problema original (passo a passo, recompõe o problema original de forma que ele faça sentido)

* _Ordem de execução:_ pode ser sequencial (geralmente um problema depende do outro, uma variável depende do outro) ou paralelo (tarefas podem ser executadas concomitantemente e depois que elas são executadas elas podem ser juntadas), depende do que precisamos

 

### _PADRÕES_

Reconhecimento de padrões envolve modelo de referência que pode determinar repetição. Reconhecemos esses padrões através de similaridades e diferenças entre os contextos.

Determinamos padrões para generalizar com o objetivo de obter resolução para problemas diferentes (esse padrão pode ser replicado para outros cenários de forma que essa resolução pode ser generalista). Fazemos isso através de classes e categorias, a partir do grau de similaridade.

A detecção de padrão vem da extração de características para a classificação de dados que é um tipo de abordagem usada. E podemos utilizar diferentes métodos com diversas aplicações, aplicações como: classificação de dados, reconhecimento de imagem, reconhecimento de fala, análise de cenas, classificação de documentos.

 

### _ABSTRAÇÃO_

Abstrair é observar, um ou mais elementos, avaliando características e propriedades separadamente (detectar características). A abstração é um processo intelectual de isolamento de um objeto da realidade (isolar da realidade). Generalizar é tornar algo geral, mais amplo, extenso.

Quando generalizamos conseguimos determinar classes e objetos que fazem parte dessas classes. Esses dados podem ser classificados por: características, pontos essenciais e generalizar x detalhar.

Abstração é muito utilizada em computação como em busca binária, merge sort e clustering, dado estruturas de dados como árvore, lista e grafos. A linguagem de programação também é uma abstração do mundo moderno para a realidade. Abstração é tornar o problema geral para conseguir utilizar em cenários distintos mas com similaridades, que tenham o mesmo padrão.

 

### _ALGORITMOS_

O computador não opera sozinho e precisa de instruções detalhadas, as quais são utilizadas através dos programas. A função do computador então é receber, manipular e armazenar os dados (processamento de dados).

O processo de resolução de problemas através de algoritmos é chamado de "step by step", utilizando as instruções que determinamos.

Para o desenvolvimento de programa precisamos:

* _Análise:_ entender e definir os dados de entrada e saída

* _Algoritmo:_ descreve o problema por meio de ferramentas narrativas, fluxograma, ou pseudocódigo

* _Codificação:_ o algoritmo é codificado de acordo com a linguagem de programação escolhida



Algoritmo são instruções passo a passo para concluir uma tarefa. Então como construir um algoritmo?

* Compreensão do problema

* Definir dados de entrada

* Definir processamento

* Definir dados de saída

* Utilizar um método de     construção

* Teste e diagnóstico

 

Para a construção de algoritmos temos:

1. _Narrativa:_ utilização da linguagem natural, sem conceitos novos e abre para diversas interpretações possíveis
2. _Fluxograma:_ utilização de símbolos pré-definidos que definem qual o tipo de ação executada, simples entendimento mas requer conhecimento prévio da estrutura
3. _Pseudocódigo:_ portugol, possui regras definidas e passos a serem seguidos, mas não é uma linguagem de programação e sim um meio termo para se acostumar com uma







# Introdução à Lógica de Programação

Lógica aplicada à programação, como um processo de pensamento atrelado ao conceito de algoritmos e resolução de problemas. Ela seria uma organização coesa, forma de raciocínio que segue convenções e fornece uma ordem para uma determinada situação. É a organização e planejamento das instruções, assertivas em um algoritmo, a fim de viabilizar a implantação de um programa.

 

*Técnicas de lógica de programação*

1. _Técnica linear:_ modelo tradicional sem vínculo (estrutura hierárquica); é uma execução sequenciada de uma série de operações, ordenação de elementos por uma única propriedade, com recursos limitados e de única dimensão
2. _Técnica estruturada:_ classificada por organização, disposição e ordem dos elementos essenciais que compõem um corpo (concreto ou abstrato), ela pode ter mais uma opção porque não é linear (mais complexa = mais vantagens)
3. _Técnica modular:_ onde determinamos partes independentes que são controladas por um conjunto de regras e cada módulo tem seu conjunto de regras específico; assim, ocorre a simplificação do algoritmo/decomposição do problema







# Fundamentos de Algoritmos

Conceitos básicos para o correto entendimento de algoritmos, como: variáveis, tipos de dados, instruções, condições, entre outros.

 

### _TIPOLOGIA E VARIÁVEIS_

A função do computador é processar as informações que damos para ele e essas informações são compostas por dois tipos: dados (objeto de manipulação) e instruções (diretivas para executar determinadas funções para processar esses dados). As instruções são as operações que tratam esses dados, e os dados são tratados e processados, e temos tipos diferentes de dados:

* _Numéricos:_ inteiros (0, 1, 800, -20) e reais (5.95, -8.8, 0, 1, 800, -20)

* _Caracteres:_ tudo aquilo que não representamos como número (que também pode ser um caractere) com aspas duplas ("programação", "KU478%8H")

* _Lógico:_ verdadeiro (1) e falso (0), está atrelado a lógica booleana onde só tem duas respostas possíveis

 

Quando queremos utilizar esses dados dentro de um programa utilizamos variáveis, que é um tipo de estrutura mutável (pode variar dentro do seu valor, pode ser sobre-escrita e modificar seu valor), e possui variações. A variável pode assumir qualquer um dos valores de um determinado conjunto de valores, contudo ela está restrita ao seu tipo (se é uma variável numérica ela vai receber números, se é string ela vai receber strings). O nome da variável segue boas práticas:

* Atribuição de um ou mais caracteres (nomes que signifiquem alguma coisa)

* Primeira letra - não número

* Sem espaços em branco

* Vedado: não utilizar palavras reservadas

* Caracteres e números

 

 

### _INSTRUÇÕES PRIMITIVAS_

Determinam as ações que iremos executar em cima dos nossos dados, que geralmente são cálculos matemáticos (para isso utilizamos os operadores), e dentro desses cálculos utilizamos como input/informação as variáveis e as constantes. Esses operadores podem ser tanto binários como unários.

Definição formal de instrução: "Instruções são linguagem de palavras-chave (vocabulário) de uma determinada programação que tem por finalidade comandar um computador que irá tratar os dados". O mesmo comando possui sintaxe distintas, as instruções primitivas dentro de cada linguagem de programação possui uma sintaxe singular.

 

### _ESTRUTURAS CONDICIONAIS E OPERADORES_

Exemplo temos uma média escolar e queremos saber se ele foi aprovado ou não. Para isso precisamos de uma estrutura condicional, onde dado o estado de uma coisa existe uma condição para aquilo acontecer. O condicional expressa uma condição ou suposição, há uma condição que se for satisfeita executa uma determinada instrução.

Em uma estrutura condicional dado uma condição que for satisfeita a operação é executada, e caso ela seja uma inverdade essa condição não é satisfeita e acarreta em uma exceção. Existem diferentes operadores relacionais que ajudam a definir as estruturas de condição dentro de um algoritmo, e se essa condição for verdadeira ele executa a ação.

Temos também os operadores lógicos e os utilizamos quando precisamos de uma resposta simplificada (verdadeiro ou falso):

* _AND:_ todas as condições devem ser satisfeitas (intersecção)

* _OR:_ apenas uma das condições deve ser verdadeira (união)

* _NOT:_ operador de negação onde a inversão do resultado lógico é o resultado (se temos uma condição que é verdadeira ela se torna falsa, se é falsa é verdadeira)

 

### _ESTRUTURAS DE REPETIÇÃO_

Quando precisamos que um pedaço do código seja executado mais de uma vez temos o laço que é um controle de fluxo, loop. Essa estrutura de repetição irá executar um determinado trecho do programa a partir de certos parâmetros que serão estabelecidos dentro dessas estruturas. Algumas de suas vantagens são a redução de linhas do programa, compreensão facilitada e redução de erro.

Existe para isso uma condição de parada, para o loop não ser infinito, como número de repetições pré-fixadas ou uma condição a ser satisfeita.

* _Enquanto (While):_ teste lógico (no início), número de repetições (indefinidas até a condição de parada ser satisfeita)

* _Repita:_ teste lógico (no final), número de repetições (indefinidas até a condição de parada ser satisfeita)

* _Para...de...até (For):_ teste lógico (no início), número de repetições (definidas)

 

 

### _VETORES E MATRIZES_

Vetor é uma sequência de dados, de tipos de dados. Pode ser visto como um container ou uma matriz. Matrizes são uma coleção de vetores, cada linha é um vetor/variável com tamanho pré-fixado e para navegarmos por esses vetores precisamos dos índices (em que linha e coluna elas estão, assim conseguimos obter as informações dela).

Um vetor é igual a um conjunto, um range, de inteiros. Essas estruturas mais complexas é melhor utilizar duas variáveis como ex. notas de diversos alunos, pega pela coluna do aluno x e a nota da prova x, isso faz ter menor quantidade de linhas.

 

 

### _O QUE SÃO FUNÇÕES?_

Funções vem da ideia da matemática e têm vários nomes: subalgoritmo, bloco, método, subprograma, sub-rotina. Uma função a partir de um elemento que ela recebe ela vai retornar um valor. Vem da parte de modularização/decomposição do problema, onde o código fica mais claro e conciso e há o aproveitamento das instruções sem repetição.

 

### _INSTRUÇÕES DE ENTRADA E SAÍDA_

Instruções de entrada consistem na inserção e recebimento de dados do mundo real por meio de ação de alguma interface, seja teclado, mouse, arquivos, entre outros. São interfaces relacionadas ao computador que permite a inserção de dados.

Instruções de saída consistem na impressão dos dados do mundo abstrato, digital por meio de ação de alguma interface. Geralmente imprimimos essas informações em uma tela, salva em um arquivo, depende. Existem dois tipos de saída: saída programada (condicional - aguarda o dispositivo para imprimir os valores - e incondicional), e saída por interrupção (definida pelos periféricos). Para toda saída existem casos: bem sucedidos, erros de sintaxe, erros de programação e problemas com a interface.







# Introdução à Linguagens de Programação

 ### _INTRODUÇÃO À LINGUAGEM DE PROGRAMAÇÃO_

É preciso falar de história da computação para compreender as dificuldades enfrentadas na época, os fundamentos da computação e o processo de pensamento. A base da tecnologia é baseado em pesquisas anteriores (lições aprendidas) e novos paradigmas.

Os problemas computacionais são recorrentes. São objetos de discussão que possuem instruções passo a passo, que se resolvem mais facilmente em ambiente computacional (problemas de decisão, de busca, de otimização) e eles se desenvolvem ao longo de cada época.

* _Problemas de decisão:_ problemas de caráter lógico, tem a ideia de pertencimento (ex.: dado um número n inteiro positivo determine se ele é primo), é decidível

* _Problema de busca:_ relacionamento binário, tem um objetivo (ex.: x está em a?)

* _Problema de otimização:_ maximizar ou otimizar uma função, aperfeiçoamento

 

 

### _COMO UM COMPUTADOR ENTENDE O PROGRAMA?_

Um código fonte é um código gerado a partir de uma linguagem de programação de alto nível, e que vai ser traduzido ou interpretado. Dado a linguagem de alto nível (como python - *programa fonte*) ele vai ser enviado para o compilador e ele vai traduzir esse programa em um código de baixo nível/linguagem de máquina (como assembly - *programa objeto*).

* _Tradução:_ há 1) geração do programa objeto e 2) execução do programa objeto, execução mais rápida, programas menores (ex.: C++, java)

* _Interpretação:_ programa fonte é executado diretamente (processo lento, porque não vai ter a compilação para o programa objeto), maior flexibilidade é uma linguagem mais fácil de se programar (ex.: ruby, python, javascript)

 

 

### _CARACTERÍSTICAS DE UM PROGRAMA_

Existem importantes características que devemos levar em conta quando programamos, como: legibilidade, facilidade de leitura, compreensão, ortogonalidade (coerência nas instruções) e definição adequada das estruturas.

 

_Redigibilidade (facilidade de escrita)_

- Pode conflitar com a legibilidade (tem que ser escrito facilmente, nem sempre isso o torna legível)
- Ortogonalidade
- Simplicidade da escrita
- Suporta à abstração
- Reuso do código
- Expressividade

 

_Confiabilidade (faz o que foi programado para fazer)_

- Verificação de tipos
- Trata exceções
- Uso de ponteiros
- Compatibilidade entre compiladores

 

_Custo (análise de impacto)_

- Treinamento
- Codificação
- Compilação
- Execução
- Infraestrutura

 

 

### _ANÁLISES E CÓDIGO_

_Análise léxica (leitura)_

- Primeira fase do processo de compilação e sua função é fazer leitura do código fonte caractere por caractere e agrupa-los em símbolos léxicos (tokens)
- Particionar (elementos léxicos = tokens - é todo elemento que é importante para a codificação do nosso programa como identificadores, números, strings), classificar (agrupa-los), eliminar (elementos como caracteres em branco, comentários)

_Análise sintática (forma)_

- Forma que o programa define qual é a estrutura relacionada para a codificação dentro daquela linguagem específica, corretude do programa
- Cada linguagem de programação vai ter uma sintaxe associada

_Análise semântica (significado)_

- Estudo do significado, é a lógica do programa
- Um erro de semântica é quando ele não faz o que é esperado

 

 

### _PARADIGMAS DE PROGRAMAÇÃO_

_O que é um paradigma_

- Forma de resolução de problemas com diretrizes e limitações específicas de cada paradigma utilizando linguagem de programação
- Possui regras para a resolução de problemas e está limitado por diretrizes/contextos específicos

_Classificação de paradigmas_

- **Orientação à objeto**
- Procedural (chamadas sucessivas e procedimentos separados)
- Funcional (instruções baseadas em funções)
- **Estruturado** (estrutura de blocos aninhados)
- Computação distribuída (funções executadas de forma independente)
- Lógico

 

_Paradigma estruturado_

- Ideia de sequência, decisão (teste lógico), iteração (funções, laços, condições)
- Instruções sendo executadas em sequência
- Ex.: C++
- Utilização: utilizado para problemas simples e diretos, aprender programação

 

_Orientação à objeto_

- Análogo ao mundo real

- Paradigma de programação baseado na utilização de objetos e suas interações

- "Um objeto é descrito por características específicas (atributos, o que eu tenho),     comportamentos (métodos, o que sou capaz de fazer) e estado (o que eu     faço)"

  

_Objeto no ponto de vista da programação_

- _POO:_ uma classe aloca em memória uma instância dessa classe (o objeto), e tem operações associadas (métodos), reuso de códigos

- _Estruturado:_ temos alocação em memória e operações associadas, essas operações estão desassociadas de uma variável, funciona com problemas específicos e diretos

  

_Pilares de orientação a objeto_

- _Herança:_ uma classe filha herda as características (atributos, métodos, comportamento) de uma classe mãe, mas ela também pode ter especializações (sobre-escrever métodos que são herdados), classe mãe tem comportamento mais geral e as classes filhas tem comportamentos mais específicos
- _Encapsulamento_
- _Polimorfismo_
- _Abstração_