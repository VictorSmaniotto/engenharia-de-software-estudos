Disciplina: Linguagens de Programação
Aula 3 - Programação Estruturada - Conceitos

Sumário[1\. Programação Imperativa](#topico-01)[

2\. Programação Estruturada

](#topico-02)[

3\. Conceitos Essenciais

](#topico-03)[

4\. Componentes de um Código

](#topico-04)

A programação possui formas alternativas de ser feita, e os paradigmas oferecem estas possibilidades, lembrando que a programação em si existe a décadas e de tempos em tempos formas alternativas foram surgindo e oferecendo novas perspectivas para o desenvolvimento de software.

## Programação Imperativa

Dentre as várias formas de programação utilizadas no desenvolvimento de software, a programação imperativa foi a inicialmente utilizada pelas linguagens de programação da época como as linguagens Algol, Fortran e COBOL, e posteriormente, as linguagens C, Basic e Pascal.

Este paradigma se baseia na mudança de estados sofrida pelos dados devido ao processamento realizado por comandos contidos no código que são executadas ao longo da execução do software.

Representa um paradigma com simples interpretação de códigos, pois os códigos são implementados dentro da premissa de indicar diretamente as ações a serem realizadas pelo hardware.

A ideia base para este paradigma foi a famosa Máquina de Turing, nomeada em homenagem ao seu elaborador, o matemático britânico Alan Turing, considerado o “pai da computação”. A máquina basicamente trabalhava com base no conjunto de hardware formado por unidade lógica e aritmética, unidade de controle, unidade de entrada e saída, e por fim, memória primária, que eram responsáveis por receber dados, processá-los e retornar resultados, criando a popular base da computação formada por entrada, processamento e saída.

A Máquina de Turing e seu desenvolvedor, Alan Turing

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a03-img01-02.jpg)

Fonte: [Disponível aqui](https://cdn.britannica.com/s:575x450/81/191581-004-95328E05.jpg)

Algumas características clássicas deste paradigma eram a construção do código como um bloco único de comandos com apenas realizando desvios dentro do código utilizando um artifício que desvia a execução com base em marcadores numéricos ou textuais inseridos no código usando um comando comumente chamado de GOTO.

Conheça a história de Alan Turing no filme “O Jogo da Imitação”. Durante a Segunda Guerra Mundial, o governo britânico monta uma equipe que tem por objetivo quebrar o Enigma, o famoso código que os alemães usavam para enviar mensagens aos submarinos aliados. Um de seus integrantes é o brilhante matemático Alan Turing (Benedict Cumberbatch).

Veja o trailer em:[Disponível aqui](https://www.youtube.com/watch?v=YIkKbMcJL_4)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

## Programação Estruturada

Uma alternativa ao paradigma imperativo desenvolvido foi a programação estruturada, que agrega os conceitos fundamentais do paradigma imperativo e acrescenta novos conceitos, definindo assim o paradigma mais popular da história do desenvolvimento de código, presente até os dias atuais em grande parte das linguagens de programação e softwares desenvolvidos.

Estruturas mais complexas são definidas, como o uso das chamadas sub-rotinas e, dentro destas, estruturas de decisão e repetição, blocos de comandos dentro de instruções que permitem a estruturação de softwares com maior complexidade e entrando no universo de linguagens de programação de alto nível.

O conceito do paradigma estruturado surgiu na década de 1950 e foi utilizado inicialmente em linguagens como Algol e COBOL, mas logo outras linguagens tiveram versões implementadas neste paradigma ou foram criadas já nativas nesta forma de programação.

Linguagens como PHP, Pearl e mais recentemente a linguagem GO desenvolvida pela Google são exemplos de linguagens que inicialmente foram desenvolvidas para desenvolvimento estruturado.

Mesmo tendo sido inicialmente pensadas como linguagens para programação estruturada, puderam ajustar-se para absorver outras formas de programação como o uso dos desvios de código do tipo GOTO em alguns casos, ou paradigmas adicionais como o orientado a objetos.

Dentro das diferentes formas de programação, é sempre bom ter alguma informação sobre os diferentes paradigmas ou formas de programação, fazendo com que se adquira maior bagagem para a definição das melhores formas e ferramentas para se desenvolver soluções computacionais. Nesta página são discutidas diferenças entre os paradigmas imperativo e declarativo que é utilizado para definir linguagens com menos estruturas lógicas como HTML e SQL onde os comandos são menos dependentes entre si em scripts criados.

Fonte:[Disponível aqui](https://pt.stackoverflow.com/questions/81854/paradigma-imperativo-e-declarativo#:~:text=A%20Programa%C3%A7%C3%A3o%20Declarativa%2C%20ao%20contr%C3%A1rio,linguagens%20definidas%20por%20este%20paradigma)

![início da abordagem prática](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-abordagem-center.svg)

## Conceitos Essenciais

Dentro da programação imperativa, o desenvolvimento de código é mais compacto e específico, em que um software projetado para um determinada finalidade, sem tanta preocupação com portabilidade ou reúso de código que representam conceitos mais atuais em que se propõe implementar código que possa ser executado em mais de uma plataforma ou sistema operacional com pouca ou nenhuma alteração de código, e também não era uma preocupação antigamente, a ideia de que partes de um software desenvolvido poderiam ser reaproveitadas no desenvolvimento de outros softwares devido a uma menor demanda e o desenvolvimento bem específico de soluções computacionais.

As estruturas de código são menos complexas e de lógica mais simples, e uma linguagem como BASIC, por exemplo, em suas primeiras versões, possuíam poucas variações de comandos. Originalmente, foi implementada com 15 tipos de comandos, suficientes para se produzir programas bastante completos em relação às necessidades computacionais da época, sendo sua facilidade de implementação de código e interpretação, motivos pelos quais se popularizou rapidamente.

Os comandos são geralmente construídos com base em uma palavra reservada da linguagem que possua uma finalidade especifica e pré-determinada da linguagem, e esta possua regras de aceite de dados adicionais chamados de parâmetros para ser construído um comando com a forma correta.

Essa forma correta de construção de cada comando se chama sintaxe e é uma das bases de qualquer linguagem de programação, sendo a linguagem BASIC uma opção com sintaxe bastante simples e intuitiva, tendo sido utilizada como primeira linguagem de programação estudada por um tempo.

A **sintaxe** é a base da construção de instruções em todas as linguagens de programação e é um mecanismo essencial para que interpretadores e compiladores possam avaliar a se é possível executar ou gerar softwares executáveis a partir de códigos escritos.

Além da sintaxe, a chamada semântica complementa o conceito de sintaxe de forma a ter um olhar mais voltado à estrutura de códigos com base nos paradigmas e implementação das linguagens para verificar se códigos estão escritos de forma adequada em suas construções lógicas e correta colocação de instruções dentro de uma estrutura compreensível por compiladores e interpretadores.

Assim, pode-se assumir de forma simplificada que a semântica se refere à **construção do código em si**, observando a correta colocação das instruções em seus devidos lugares, estejam elas corretas ou não, pois essa outra preocupação é função da sintaxe.

Dentro dos conceitos fundamentais, ainda é importante deixar mais claro a diferença entre os processos realizados na análise de código para posterior execução, e entram então os conceitos de compilação e interpretação.

A **compilação** é um processo realizado em partes em que um código fonte escrito é analisado e primeiramente uma das principais etapas reúne os caracteres para a construção de lexemas, ou conjuntos de caracteres reconhecidos como palavras reservadas, identificadores (nomes em geral), valores numéricos, etc., a fim de facilitar etapas posteriores do processo, e ai se compreende a necessidade de uma correta digitação de códigos fonte.

Segundo Sebesta (2011), em outra etapa, outro componente chamado de **analisador sintático** utiliza as unidades léxicas criadas a partir do código fonte para estruturar as chamadas árvores léxicas que servem para que se possa analisar se comandos foram escritos de forma adequada com a correta colocação de palavras reservadas e parâmetros obrigatórios ou opcionais possíveis.

Outra etapa, um processo de análise semântica, preocupa-se com a estrutura toda do código avaliando instruções completas e sua correta colocação dentro da lógica de programação da linguagem utilizada.

Este conjunto de etapas e outros processos realizados são a base para a transformação de um código fonte escrito e legível para um novo conteúdo em arquivo chamado objeto, intermediário no processo todo que elimina elementos desnecessários em um código fonte como comentários, e já tendo sua estrutura avaliada e preparada para os próximos passos.

Numa etapa posterior, o chamado “linkador” tem a função de agregar ao arquivo objeto intermediário, bibliotecas e demais elementos externos chamados pelo código fonte para que juntos se tornem um único bloco que representa o software em si executável, já todo verificado e funcional.

Erros de codificação são verificados, mas nem todo tipo de erro é possível de ser validado pelo processo, pois há casos onde erros na lógica ou de uso incorreto de comandos para determinadas ações não pode ser identificado na etapa de compilação, mas somente na execução e teste, pois são mais perceptíveis nestes momentos.

Já no processo de **interpretação**, o código fonte é analisado, avaliado e executado diretamente por uma ferramenta como um navegador ou interpretador que não gera software executável, mas apenas executa o código fonte sequencialmente, e este processo pode agir de duas formas.

Erros contidos no código que possam ser ignorados são descartados durante a execução, como ocorre comumente em páginas web exibidas em navegadores, em que alguns comandos com erros deixam de ser executados e parte do conteúdo a ser exibido em uma página simplesmente não aparece, sem impedir a exibição dos demais elementos se possível.

Outro tipo de interpretação realiza todo o processo de análise prévia do código antes da interpretação de forma a executar o código apenas se este estiver estruturado de forma correta sintática e semanticamente, como no processo de compilação, tanto que arquivos temporários intermediários podem ser gerados para que a interpretação seja realizada a partir deles.

Num terceiro tipo de processo, a compilação ocorre, mas um software executável independente de outras ferramentas não é gerado, parando então a execução na geração do arquivo objeto intermediário, como ocorre na linguagem Java em que se cria um código fonte e este é então convertido em arquivo de um tipo chamado de Bytecode que é depois, interpretado por um software conhecido como máquina virtual.

Esse chamado arquivo **bytecode** (objeto) é portável e pode ser geralmente executado em qualquer plataforma, desde que ela possua um interpretador próprio para este tipo de bytecode instalado, permitindo então que um mesmo código possa ser executado nestas diferentes plataformas (sistemas operacionais e tipos de hardware) sem alteração se possível, permitindo alta portabilidade de código na linguagem Java.

Essa portabilidade é reduzida em linguagens compiladas, pois além das especificidades de cada plataforma, os compiladores geralmente não são os mesmos e um mesmo código fonte deve ser compilado em cada plataforma para a geração de softwares executáveis que não podem ser executados em outras plataformas sem o uso de emuladores ou simuladores de ambientes de plataformas.

## Componentes de um Código

Na estruturação de código fonte em linguagens para programação estruturada, são utilizadas estruturas variadas para compor soluções computacionais para que o processamento de dados possa ser realizado e problemas de complexidades variadas possam ser resolvidos.

Geralmente, as linguagens de programação estruturadas permitem a construção de instruções contendo blocos de comandos, e estas instruções representam a base da codificação englobando estruturas para realização de desvios condicionais e laços de repetição que serão trabalhados com exemplos na aula 04.

Também serão demonstradas a declaração e o uso de estruturas de dados variadas como variáveis que representam unidades simples de armazenamento de dados, e estruturas mais complexas como matrizes de dados, por exemplo.

Outro conceito relevante é o de subdivisão de códigos em sub-rotinas que permitem maior possibilidade de reúso de código, independência entre partes de um código, e melhor legibilidade e facilidade de leitura e compreensão de código.

Geralmente, ainda existe a possibilidade de inclusão de funcionalidades prontas armazenadas em arquivos contendo código chamadas de bibliotecas de forma geral, que auxiliam no desenvolvimento de software em menor tempo utilizando funcionalidades já desenvolvidas e testadas como para ações de entrada e saída de dados padrão.

Assim, a ideia geral do estudo desta disciplina é que sejam apresentados conceitos ligados ao desenvolvimento de soluções computacionais para solução de problemas a partir da abstração destes problemas e avaliação de algoritmos a serem posteriormente implementados em linguagens que possam oferecer melhor custo e benefício a partir de vários aspectos analisáveis.

Veja exemplo de programa em linguagem BASIC na imagem a seguir, em que as linhas numeradas são fundamentais como referência para os desvios do fluxo de execução realizados pelo comando GOTO que se referência a elas para este processo.

**10 REM EXEMPLO DE PROGRAMA EM BASIC - DIVISÃO**

**20 READ A**

**30 READ B**

**40 IF B=0 THEN GOTO 200**

**50 LET C=A/B**

**60 PRINT "RESULTADO DA DIVISÃO: ",C**

**70 PRINT “DESEJA REALIZAR OUTRO CÁLCULO (S/N)?”**

**80 LET D**

**90 IF D=”S” THEN GOTO 20**

**100 IF D=”N” THEN GOTO 300**

**110 GOTO 70**

**200 PRINT “O DIVISOR NÃO PODE SER ZERO!”**

**210 GOTO 30**

**300 END**

Também é interessante analisar o fluxo de execução em si em que são solicitados valores para as variáveis A e B, e caso B seja zero, é desviado o fluxo para um tratamento desta exceção na linha 200 informando o usuário e retornando a linha 30 para a inserção de novo valor.

Depois, é realizada a operação e exibido o resultado ao usuário que tem, em seguida, a opção por realizar ou não outra divisão, resultando nas possibilidades de desvio para a linha 20 para novo cálculo, desvio para a linha 300 para encerramento e desvio para a linha 70 caso seja digitada uma opção inválida.

!

### Nesta aula estudamos:

- Programação Imperativa
- Programação Estruturada
- Conceitos Essenciais
- Componentes de um Código
