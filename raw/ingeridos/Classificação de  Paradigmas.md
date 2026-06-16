Disciplina: Linguagens de Programação
Aula 2: Classificação de Paradigmas

Sumário[1\. Categorias de Linguagens de Programação](#topico-01)Os paradigmas de programação representam formas variadas de se desenvolver soluções computacionais e as linguagens de programação são ferramentas para tal atividade baseadas nestes paradigmas, sendo que algumas linguagens podem utilizar conceitos de mais de um paradigma integrando estes conceitos com o propósito de oferecer soluções mais completas e atender uma maior gama de problemas.

Geralmente, as linguagens de programação são criadas com objetivos previamente definidos como para o desenvolvimento de softwares científicos como no caso da linguagem Fortran, ALGOL e Assembly que possuem capacidade de tratar cálculos complexos de ponto flutuante, ou seja, cálculos com casas decimais.

Também existem linguagens como COBOL criadas para o desenvolvimento de softwares comerciais, linguagens como Lisp, Prolog e Scheme para desenvolvimento na área de IA (Inteligência Artificial), linguagens como C para a programação de SO (Sistemas Operacionais) por serem altamente capazes de manipular hardware mesmo sendo de alto nível, e linguagens como PHP e JavaScript para desenvolvimento de conteúdo para web.

Segundo Sebesta (2011), as linguagens de programação podem ser avaliadas segundo alguns critérios como legibilidade de seus códigos, facilidade na escrita destes e a confiabilidade dos softwares desenvolvidos a partir de cada linguagem. Observe a figura 3 para conhecer estes critérios e suas características relevantes.

Imagem 3: Critérios e características de linguagens de programação.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a02-figura01.svg)

Fonte: Sebesta, 2011.

Algumas características citadas são realmente fundamentais na avaliação de uma linguagem como a simplicidade que é importante nos três critérios de avaliação, pois sendo simplificada, torna seus códigos mais fáceis de compreender e implementar, tendo pouca variedade de estruturas básicas de programação.

Outra característica importante é a ortogonalidade que toma por base a quantidade de combinações entre estruturas de dados e de controle, reduzindo a possibilidade de ambiguidades e exceções, tornando uma linguagem mais compacta e com menor possibilidade de ocorrência de erros devido a exceções. Linguagens como C, por exemplo, permitem que sejam utilizados ponteiros que são operadores de tipo que trabalham com a memória em hardware de diversas formas, reduz a ortogonalidade da linguagem devido à grande possibilidade de combinações possíveis destes operadores e tipos da linguagem.

Outra característica importante se refere aos tipos de dados e estruturas possíveis em uma linguagem que podem facilitar ou dificultar os critérios base de avaliação de uma linguagem, como no caso da linguagem C que não possui tipo lógico e utiliza valores numéricos de forma adaptada para esta funcionalidade, não sendo um defeito da linguagem, mas apenas uma característica que dificulta a legibilidade de códigos e sua interpretação clara muitas vezes.

Por fim, outra característica presente em todos os critérios se baseia no projeto da sintaxe de cada linguagem, e segundo Sebesta (2011), o formato definido como padrão de definição de identificadores, palavras reservadas da linguagem e seu uso na construção de estruturas de controle de fluxo no código, e a forma como se implementa uma instrução na linguagem possui influência direta em sua legibilidade também.

Dentro do critério de facilidade de escrita e confiabilidade, existe ainda a preocupação com o suporte à abstração que se refere a capacidade de definir em processos e estruturas de dados as características relevantes de um problema real.

Também existe a chamada expressividade que está presente na análise de facilidade de escrita e confiabilidade que se refere a aspectos como a simplificação de expressões e existência de comandos que facilitem a codificação como a existência de mais de um comando para implementação de laços de repetição, por exemplo.

Mais especificamente voltadas à confiabilidade, existem características como a verificação de tipos durante o processo de compilação de um código que é melhor que em tempos de execução em relação a custo de processamento, tratamento de exceções para melhoria da garantia de funcionamento de softwares, uso de apelidos ou alias que servem para acessar uma mesma posição de memória como no uso de ponteiros em linguagens como C, e por fim, a própria legibilidade e facilidade de escrita influenciam a confiabilidade de um código.

Compreender a estrutura de um algoritmo ou código de uma linguagem de programação é o primeiro passo essencial para se aprender a programar, mas antes ainda, é preciso aprender a interpretar problemas e deles obter informações capazes de auxiliar no início do esboço da lógica de uma provável solução computacional.

![início da abordagem prática](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-abordagem-center.svg)

## Categorias de Linguagens de Programação

Linguagens mais antigas eram criadas especificamente para determinados hardwares e o conceito de paradigmas de programação foi sendo definido ao longo dos anos para diferenciar as diferentes abordagens da implementação de software.

As três principais categorias de linguagens de programação (Sebesta, 2011) são imperativas, funcionais e lógicas, mas existe uma derivação vinda da programação imperativa chamada de orientação a objetos.

Pode-se subcategorizar as linguagens de programação em ramificações das categorias principais como no caso das linguagens que gerar scripts como JavaScript, Ruby e Perl, mas estas são basicamente imperativas.

Linguagens voltadas a interfaces gráficas foram desenvolvidas depois de muitas outras, mas são geralmente baseadas em alguma linguagem mais antiga e originalmente de modo textual como C, Basic ou Pascal que geraram versões para interfaces gráficas como Visual-C, Visual Basic e Delphi, além das ditas linguagens visuais como Visual BASIC.NET (VB.NET) (Sebesta, 2011).

A programação lógica, baseada em regras define seus programas de forma distinta da imperativa, pois as regras que servem da base são definidas sem uma ordem lógica e podem ser acessadas livremente de forma que sirvam como uma base complexa de informações que podem ser utilizadas na geração de novas informações.

Numa linguagem imperativa, existe uma ordem lógica para a execução de uma grande variedade de estruturas que podem ser organizadas como independentes ou dependentes umas das outras, mas tendo uma ordem planejada de execução.

As linguagens funcionais trazem uma perspectiva mais matemática para a programação com dados constantes e funções de comportamento fixo que facilita a reutilização e ampliação de aplicações de forma escalar em função da não mutabilidade destas funções.

A programação orientada a objetos possui foco na abstração de dados estruturando-os como atributos de classes que são evoluções das funções em programação imperativa e permitem uma maior independência entre estes componentes que acabam sendo mais facilmente reutilizados em novos softwares.

Além da divisão dos paradigmas nestas quatro diferentes linhas de programação, algumas outras variantes surgem como propostas como propostas de variações da orientação a objetos, por exemplo, como a programação orientada a eventos ou orientada a aspectos, ou formas alternativas de programação como em linguagens que podem ser consideradas declarativas como HTML e SQL, ou linguagens de programação baseadas em blocos como Scratch e Blocky.

Existem também métodos complementares como a programação dinâmica que busca quebrar problemas mais complexos em outros de menor complexidade que trabalham com grafos, por exemplo.

Nesta ideia da programação dinâmica, este processo de resolução de subproblemas precisa ser bem pensado para que depois, estes subproblemas possam ser integrados e uma solução computacional funcional e completa seja obtida.

A ideia de problemas relacionados a custos de rotas e a obtenção dos melhores resultados é um típico problema que pode ser solucionado com este método que trabalha com entradas de dados que influenciam dinamicamente o processamento e assim, este método é capaz de gerar mudanças na execução em função destas entradas de dados por eventos que podem influenciar processos.

Este método trabalha com um conceito importante que será mais bem explorado mais adiante no material chamado de recursividade, onde trechos de código são chamados repetidamente por eles mesmos, realimentando o trecho com novos dados até que determinada condição encerre este processo.

Existem algoritmos que tratam de uma lógica mais complexa e evoluída do uso de sub-rotinas capazes de chamarem a si mesmas de forma iterativa ou repetitiva, também chamada de recursiva, onde existe um controle da quantidade de iterações baseado em uma condição que muitas vezes envolve valores numéricos que ao serem atingidos, encerram as sucessivas chamadas à sub-rotina e as seguidas repetições.

Cada paradigma, assim como cada linguagem de programação possui recursos que auxiliam no desenvolvimento de determinados tipos de software, como os tipos de estruturas de dados que utilizam e a forma como as manipulam, sua capacidade de lidar diretamente com hardware ou não, serem compiladas ou interpretadas, etc. Estas especificidades de cada linguagem apoiadas nos paradigmas que elas usam como base permitem que os desenvolvedores tenham opções mais adequadas para cada tipo de problema a ser solucionado. Algumas linguagens se propõem a serem de propósito geral como C++ e Java, e outras mais específicas como Haskell e Prolog, mas todas podem ser aplicadas e o mercado possui espaço para que saiba codificar em muitas destas linguagens, lembrando que o bom programador não é aquele que conhece várias linguagens, mas aquele que sabe pensar em bons algoritmos eficientes e conhece uma boa linguagem para aplicar a estes algoritmos.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Outro paradigma chamado de funcional se baseia em sub-rotinas que executam processos como se fossem funções matemáticas em que se evitam ao máximo mudanças de estado ou dados dinâmicos que são características comuns nos paradigmas imperativo e estruturado que utilizam muitas estruturas de dados variáveis e estados que mudam o tempo todo na execução.


- Categorias de Linguagens de Programação
