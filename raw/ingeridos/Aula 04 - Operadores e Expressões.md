---
title: "Aula 04 - Operadores e Expressões"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-04.html"
author:
published:
created: 2026-05-28
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 04 - Operadores e Expressões

Sumário[1\. Fundamentos de Lógica para Programação](#topico-01)[

2\. Operadores Matemáticos

](#topico-02)[

3\. Operadores Relacionais

](#topico-03)[

4\. Operadores Lógicos

](#topico-04)[

5\. Expressões Matemáticas e Lógicas

](#topico-05)[

6\. Precedência de Operadores

](#topico-06)

## Fundamentos de Lógica para Programação

Para se desenvolver algoritmos que representam formas de se resolver problemas reais de modo computacional, é preciso que se compreenda que além de imaginar uma sequência de instruções para realizar tarefas, é preciso uma compreensão do problema a ser resolvido e se é ou não possível que se elabore uma solução computacional para o problema em questão de forma completa ou parcial ao menos.

Interpretar problemas e avaliar situações é muito importante, assim como prever situações e elaborar meios para que um algoritmo possa conter as funcionalidades desejadas.

Muitas vezes é preciso realizar cálculos, avaliar situações e escolher diferentes fluxos na execução de algoritmos de forma que este seja capaz de realizar atividades variadas dentro das limitações que possam existir nos algoritmos.

Para a elaboração de algoritmos, existem diversas regras e definições que precisam ser seguidas para que os algoritmos criados sejam todos padronizados e existem muitos símbolos com finalidades específicas como cálculos, por exemplo, assim como palavras que são utilizadas na elaboração e devem ser “reservadas” para uso apenas como comandos, sendo que demais palavras utilizadas representam outros elementos que serão aos poucos estudados.

## Operadores Matemáticos

A utilização de operadores matemáticos é semelhante ao seu uso na matemática e representam diferentes cálculos, mas alguns símbolos são diferentes em função da limitação de símbolos existentes no teclado, visando facilitar sua identificação em meio a um algoritmo que pode conter muitos elementos distintos.

Os operadores matemáticos utilizados na elaboração de algoritmos são os mais comuns, pois em geral são utilizados na grande maioria dos algoritmos, e por isto, são aqueles implementados geralmente nas linguagens de programação. Observe a seguir os operadores mais utilizados e sua finalidade.

| **OPERADOR** | **DESCRIÇÃO** |
| --- | --- |
| + | Operador soma. |
| \- | Operador subtração. |
| \* | Operador multiplicação. |
| / | Operador divisão. |
| % | Operador resto da divisão. |

Tabela 2: Operadores matemáticos | Fonte: O autor.

A partir da observação da simbologia utilizada na tabela 1, é possível perceber que os símbolos matemáticos para soma e subtração permanecem os mesmos, mas o símbolos utilizados para multiplicação e divisão são alterados para os símbolos “\*” e “/” em função do uso constante da letra X e do símbolo “:” e da ausência do símbolo “÷”.

O símbolo “%” que é utilizado como operador resto da divisão entre dois valores serve para devolver como resposta o valor restante de uma divisão com resultado inteiro apenas. O uso para estruturação de cálculos em geral segue a mesma e será demonstrado posteriormente no estudo de expressões.

## Operadores Relacionais

Outro tipo de operador se chama relacional, pois estabelece relação entre dados que resultam em valores verdadeiro ou falso, sendo muito utilizado como meio para a tomada de decisão para desvios na execução ou repetições de processamento, por exemplo.

Estes operadores envolvem o uso de raciocínio lógico para seu emprego, diferente dos operadores matemáticos que necessitam apenas que se saiba qual o tipo de cálculo realizado por cada um. A tabela 3 traz os operadores relacionais padrão para algoritmos.

| **OPERADOR** | **DESCRIÇÃO** |
| --- | --- |
| \> | Maior. |
| \>= | Maior ou igual. |
| < | Menor. |
| <= | Menor ou igual. |
| \= | Igual. |
| <> | Diferente. |

Tabela 3: Operadores relacionais | Fonte: o autor.

Os símbolos contidos na tabela 3 são praticamente os mesmos da matemática, com exceção do símbolo “<>” que é utilizado ao invés do símbolo “≠” em função da ausência do mesmo no teclado. Existem linguagens de programação que utilizam simbologia diferente para este operador.

## Operadores Lógicos

Existem várias operações lógicas utilizando operadores distintos para comparações que resultam sempre em valores verdadeiro ou falso, assim como os operadores relacionais, mas seu uso é diferente dos operadores relacionais.

Enquanto os relacionais comparam dois dados, os operadores lógicos são utilizados para comparações compostas, em que são definidas regras para o uso destes operadores e a forma como podem ser utilizados em linguagens de programação.

Os operadores básicos lógicos utilizados na elaboração de algoritmos são E, OU e NÃO, mas existem outros que podem ser estudados como NOR, NAND e XOR, por exemplo. Observe a imagem 8 que traz um meio de se compreender o uso destes operadores.

<table><tbody><tr><th><strong>Expressão A</strong></th><th><strong>Expressão B</strong></th><th><strong>OPERADOR E</strong></th></tr><tr><td>V</td><td>V</td><td>V</td></tr><tr><td>V</td><td>F</td><td>F</td></tr><tr><td>F</td><td>V</td><td>F</td></tr><tr><td>F</td><td>F</td><td>F</td></tr><tr><th><strong>Expressão A</strong></th><th><strong>Expressão B</strong></th><th><strong>OPERADOR OU</strong></th></tr><tr><td>V</td><td>V</td><td>V</td></tr><tr><td>V</td><td>F</td><td>V</td></tr><tr><td>F</td><td>V</td><td>V</td></tr><tr><td>F</td><td>F</td><td>F</td></tr><tr><th colspan="2"><strong>Expressão A</strong></th><th><strong>OPERADOR E</strong></th></tr><tr><td colspan="2">V</td><td>F</td></tr><tr><td colspan="2">F</td><td>V</td></tr></tbody></table>

Imagem 8: Tabelas-verdade | Fonte: o autor.

Por meio do conhecimento das tabelas-verdade de cada operador lógico, é possível compreender sua aplicabilidade e interpretar o que ocorre na aplicação destes operadores em algoritmos.

O operador E age como se, para que seu resultado seja verdadeiro, as expressões analisadas devem ser todas verdadeiras, sem nenhum valor falso que invalide este operador.

O operador OU possui maior facilidade em retornar verdadeiro, pois se pelo menos um dos dados ou expressões avaliados sejam verdadeiros, já é suficiente para que um retorno verdadeiro seja obtido.

Por fim, o operador NÃO apenas inverte o valor verdadeiro ou falso contidos em uma estrutura de dados e pode ser útil em diversas situações relativas à inversão de estados em um algoritmo. Mais adiante serão criados alguns exemplos utilizando estes tipos de operadores.

A compreensão dos operadores lógicos e sua variedade é algo importante para o desenvolvimento de algoritmos, pois podem ser utilizados em diversas situações em que são realizadas tomadas de decisão baseadas em expressões lógicas.

Acesse o link:[Disponível aqui](https://www.todamateria.com.br/tabela-verdade/)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Expressões Matemáticas e Lógicas

O uso de operadores é muito comum em algoritmos. E expressões de tipos variados podem compor uma solução que não precisa ser necessariamente voltada à realização de cálculos, pois além dos operadores matemáticos, existem os operadores relacionais e lógicos, voltados à elaboração de comparações.

Expressões matemáticas são geralmente elaboradas com valores e operadores matemáticos, mas para obedecerem à forma como uma instrução que use expressões matemáticas, a chamada sintaxe deve ser obedecida, mantendo uma padronização na estrutura de algoritmos.

Já os operadores relacionais e lógicos costumam ser utilizados em condições de estruturas de controle do fluxo de execução do algoritmo e complementam comandos intermediados por condições a serem avaliadas durante a execução. Observe os exemplos da imagem 9.

SOMA <- 3 + 5;

MEDIA <- (VALOR1 + VALOR2) / 2;

RESULTADO <- 5 + (3 \* 2 – (1 + 4));

SE (IDADE > = 18) ENTÃO

SE (VALOR > 0 E VALOR < 10) ENTÃO

Imagem 9: Exemplo de expressão matemática | Fonte: O autor.

Nestes exemplos da imagem 9, existem alguns pontos de atenção, como, por exemplo, a inclusão do símbolo “<-“ que representa uma atribuição de dados a uma estrutura de dados para que possa este valor ficar temporariamente armazenado para uso posterior do algoritmo enquanto está sendo executado.

Em relação às instruções em si, a primeira traz uma soma simples entre dois valores numéricos inteiros, em que o resultado será inserido na estrutura chamada de “SOMA”. Na sequência, a estrutura “MEDIA” receberá o resultado do cálculo da soma dos dois dados contidos nas estruturas valor1 e valor2, que após a soma, devem ser divididos por 2, pois a operação realizada primeiro é a contida nos parênteses.

Depois, uma expressão mais complexa é posta como exemplo, em que os cálculos entre parênteses são realizados antes dos demais, mas como há dois níveis de parênteses, o mais interno é calculado antes, para depois os parênteses mais externos e, por fim, os demais cálculos restantes.

Nos dois últimos exemplos, são utilizadas instruções de controle para exemplificar a inclusão de condições utilizando operadores relacionais e lógicos, em que em um, a condição retorna verdadeira apenas se o dado contido na variável “IDADE” for maior ou igual a 18. E no outro exemplo, são usadas duas condições relacionais, mas que pelo uso do operador “e”, devem ser consideradas juntas, pois apenas as duas sendo verdadeiras é possível a obtenção de um resultado verdadeiro.

Desde os estudos da matemática até a elaboração de instruções de controle de fluxo da execução de algoritmos, expressões matemáticas, relacionais e lógicas são utilizadas frequentemente na implementação de algoritmos, pois permitem que os algoritmos tenham a capacidade de tomada de decisões a partir de resultados obtidos nestas expressões.

A automatização proporcionada por algoritmos em equipamentos e máquinas de todos os tipos avança há décadas, e muito dessa possibilidade de evolução tecnológica se baseia na programação da máquina a partir do *software* que possui em si vários mecanismos capazes de avaliar dados e realizar ações a partir de resultados obtidos em expressões.

Por isso, é essencial ao desenvolvedor ser capaz de elaborar expressões diversas utilizando operadores e sendo capaz de avaliar as possibilidades resultantes destas expressões.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg)

## Precedência de Operadores

Com tantos operadores disponíveis é comum que vários sejam utilizados em uma mesma expressão, e assim, é preciso que seja determinada uma ordem para que estes operadores sejam executados de forma padronizada, seguindo os princípios da matemática principalmente.

Pela regra geral, a multiplicação, divisão e resto são prioritárias sobre soma e subtração, mas o uso de parênteses pode mudar avaliação natural e operações mais fracas podem ser realizadas antes de operações de maior prioridade.

Os operadores relacionais possuem todos os mesmos níveis de prioridade e só são executados após os operadores matemáticos, pois como trabalham com análises de veracidade de expressões, é importante terminar os cálculos e após, verificar se o resultado é verdadeiro ou falso.

No exemplo da imagem 13, por exemplo, a expressão que serve de base para uma estrutura “RESULTADO <- 5 + (3 \* 2 – (1 + 4));” deve ser calculada primeiramente (1+4) por serem os parênteses mais internos, para depois serem realizadas as operações dos parênteses mais externos, e neste, há uma multiplicação e uma subtração. Neste caso, primeiro multiplica-se 3 \* 2, para depois ocorrer a subtração do valor obtido na multiplicação pelo valor resultante dos parênteses internos. Com isto, o valor gerado para alocação em memória seria 6, nesta expressão exemplo.

Imagem Ilustrativa

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a04-img1.jpg)

A precedência de operadores é fundamental para a lógica de algoritmos ser correta, mas para isto é importante conhecer a finalidade de cada tipo e operador específico e a partir da construção de expressões diversas mudando operadores e adicionando ou removendo parênteses, testar resultados a partir do ajuste da precedência.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Fundamentos de Lógica para Programação
- Operadores Matemáticos
- Operadores Relacionais
- Operadores Lógicos
- Expressões Matemáticas e Lógicas
- Precedência de Operadores

Para complementar seus estudos, assista à videoaula a seguir: