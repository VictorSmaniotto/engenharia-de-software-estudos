---
title: "Aula 08 - Estruturas de Repetição"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-08.html"
author:
published:
created: 2026-05-28
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 08 - Estruturas de Repetição

Sumário

## Estruturas de Controle

Também existem estruturas que permitem que uma instrução ou conjunto de instruções sejam executados repetidas vezes de uma forma controlada para que determinadas situações encerrem as repetições, se desejado.

Este tipo de estrutura é bastante útil e permitiu que uma significativa redução na quantidade de linhas de algoritmos fosse obtida em função de ações repetitivas não mais necessitarem ser escritas diversas vezes em sequência.

A ideia de um laço de repetição é a execução de um trecho de código repetidas vezes, mas é importante deixar claro que a repetição não precisa ser necessária e exatamente das mesmas instruções.

É possível inserir, por exemplo, estruturas de decisão usando os comandos “SE” e “ESCOLHA” sem problemas em estruturas de repetição, obtendo assim, algoritmos de uma maior complexidade e capazes de realizar processamento automatizado, repetitivo e com tomada de decisão automática.

O princípio básico do uso de estruturas de repetição é a repetição de trechos de algoritmos para que certo conjunto de instruções seja repetido certo número de vezes, mas é comum que certos algoritmos sejam praticamente inteiros inseridos em uma estrutura de repetição, pois toda a sua funcionalidade é repetitiva e a própria estrutura de repetição mantém o algoritmo funcionando até que se decida encerrá-lo pela condição estabelecida para a continuidade da repetição.

Quando uma estrutura de repetição entra em funcionamento, seguidas iterações das instruções contidas na estrutura ocorrem até que determinada condição falhe e o laço seja encerrado, e este pode ser pré-determinado ou ser controlado pelo andamento da execução do algoritmo.

## Estruturas de Repetição Condicional

Um tipo de estrutura de repetição bastante usado inicia com a verificação de uma condição para avaliar se as instruções contidas neste devem ser executadas ou não, e para isto, uma condição deve ser elaborada logo na primeira linha de comando da instrução.

Esta condição deve ser responsável por verificar a cada iteração, se o laço de instruções deve continuar sendo executado, ou se as mudanças ocorridas no decorrer da iteração alteraram o estado dos dados que são verificados na condição da estrutura e tornam o resultado da expressão condicional falso, encerrando-o.

Um exemplo de estrutura de repetição condicional em que a verificação do laço ocorre logo no início da instrução de controle é mostrado na imagem 22. Observe a forma como a lógica para a estrutura é elaborada de forma que após certa quantidade de vezes, o laço é encerrado automaticamente.

CONTADOR <- 1;

ENQUANTO (CONTADOR < = 100) FAÇA

ESCREVA (“ITERAÇÃO “, CONTADOR);

CONTADOR <- CONTADOR +1;

FIMENQUANTO;

Imagem 22: Exemplo de estrutura de repetição condicional. | Fonte: O autor.

Neste exemplo da imagem 22, é definida uma estrutura de repetição que utiliza uma variável “CONTADOR” para servir de base para a expressão condicional para repetição de iterações no laço definido com duas instruções a serem repetidas.

A condição verifica antes mesmo de a primeira iteração ocorrer, se o valor contido na variável “CONTADOR” é maior ou igual a 100, condição esta que define que enquanto o valor da variável for menor ou igual ao valor definido na condição, as iterações devem continuar seguidamente ocorrendo.

Alguns detalhes muito importantes neste exemplo da imagem 22 são inicialmente para reduzir riscos na execução adequada da estrutura, a variável “CONTADOR” recebe um valor zero para sua inicialização, pois pode ocorrer de haver algum valor inesperado na variável antes da verificação da condição que poderia prejudicar a execução adequada do laço de repetição ou até impedir seu início em caso de valor maior que 100.

Ilustrativa | Fonte: martinholv

[Disponível aqui](https://elements.envato.com/pt-br/codigo-no-software-de-programacao-de-tela-do-HYSWVPH)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a08-img1.jpg)

Outro detalhe importante é que dentro do próprio laço de repetição é preciso criar condições para que a situação que torna falsa a expressão de validação de continuidade do laço de repetição aconteça se for desejado, pois caso contrário, o laço de repetição se repete infinitas vezes e isso pode não ser uma premissa do algoritmo.

Por último, é importante observar que a variável “CONTADOR” foi inicializada com o valor 1, mas este valor varia de acordo com a lógica do algoritmo e pode ser qualquer outro valor, da mesma forma que o valor da condição que define quando o laço deve ser interrompido e a forma como o valor da variável de controle é ajustada a cada iteração.

Em um segundo exemplo postado na imagem 23, outra forma de uso de laços de repetição é trazida para agregar novas ideias de como elaborar uma estrutura de repetição.

CONTADOR <- 1;

REPITA

ESCREVA (“ITERAÇÃO “, CONTADOR);

CONTADOR <- CONTADOR + 1;

ATÉ (CONTADOR > 100);

Imagem 23: Exemplo de estrutura de repetição condicional. | Fonte: O autor.

Aqui no exemplo da imagem 23, ocorre uma mudança que aparentemente afeta pouco o algoritmo em si, comparando-o com o exemplo da imagem 23, mas na verdade esta pequena mudança faz toda diferença muitas vezes.

O detalhe mais importante a ser observado para este exemplo é o que acontece com a condição que verifica se as iterações devem continuar ocorrendo ou não. Houve uma mudança de posição da expressão que avalia esta decisão e ela foi posicionada ao final da instrução que controla a estrutura de repetição.

Além disso, é muito importante observar que a lógica para este exemplo foi alterada em relação à construção da expressão de avaliação, pois foi necessária uma modificação na expressão condicional para que, ao invés de ser verificado se o valor da variável “CONTADOR” é menor ou igual a 100 para que o laço de repetição seja interrompido, agora, é verificado se o valor é maior que 100 como condição para que as iterações continuem ocorrendo.

O uso de estruturas de repetição é bastante importante e permite que algoritmos realizem tarefas repetitivas com menos código. A escolha adequada entre as opções depende de preferências do programador, mas também é influenciada pelo tipo de processamento a ser realizado e da condição para que tal ocorra.

Acesse o link:[Disponível aqui](http://uab.ifsul.edu.br/tsiad/conteudo/modulo1/lop/lop_ud/lop_04.html)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Estruturas de Repetição Contada

Outro tipo de estrutura de repetição se baseia na possibilidade de se estabelecer previamente a quantidade de iterações que devem ocorrer logo na composição do comando de controle da estrutura de repetição.

Este controle é feito indicando uma variável para controle das iterações a partir de uma regra definida no próprio comando, indicando o valor inicial para a variável de controle, uma condição de continuidade das iterações e a forma como o valor da variável de controle vai sendo afetado a cada iteração.

A construção do comando pode ser feita de formas alternativas, mudando inclusive a proposta inicialmente citada, mas a princípio será tratada a estrutura de repetição contada como uma estrutura com a predefinição da quantidade de iterações na própria construção do comando.

Para isso, utiliza-se a palavra reservada “PARA” que na forma a ser estudada inicialmente, recebe três parâmetros que definem, respectivamente, um valor inicial para a variável de controle, depois o valor final para a variável de controle que definirá um valor final para a quantidade de iterações, e por fim, uma regra para incremento ou decremento do valor da variável de forma a partir do valor inicial, e após certo número de iterações, o valor final ser atingido. Observe o exemplo da imagem 24.

PARA CONTADOR DE 1 ATÉ 100 PASSO 1 FAÇA

ESCREVA (“ITERAÇÃO “, CONTADOR);

FIMPARA;

Imagem 24: Exemplo de estrutura de repetição contada. | Fonte: O autor.

No trecho de algoritmo da imagem 24, foi criada uma versão alternativa para a estrutura de repetição do exemplo da imagem 23 em que é possível primeiramente observar uma grande redução na quantidade de linhas de algoritmo necessárias para se obter uma mesma funcionalidade.

Um dos motivos para a redução foi a não necessidade de se inserir duas linhas de algoritmo extras para controle da variável “CONTADOR”, pois todo o controle da estrutura de repetição é definido no comando principal da instrução.

O comando é construído inicialmente pela palavra reservada “PARA” e em seguida, pela variável de controle “CONTADOR”. Depois a palavra reservada “DE” indica um valor inicial para a variável de controle.

Na sequência, a palavra reservada “ATÉ” contém um valor que serve como condição de parada para o laço de repetição, seguido da palavra reservada “PASSO” que define a regra de alteração do valor da variável “CONTADOR” a cada iteração. Por fim, a palavra reservada “FAÇA” inicia o conjunto de instruções que podem estar contidas no laço de repetição.

Após as instruções inseridas na estrutura de repetição, encerra-se a estrutura com a palavra reservada “FIMPARA”, assim como no laço de repetição “ENQUANTO” utiliza-se a palavra reservada “FIMENQUANTO”.

Em muitas linguagens de programação é possível controlar uma estrutura de repetição do tipo contada “PARA” de forma semelhante às citadas nas estruturas de repetição condicionais “ENQUANTO” e “REPITA”.

Para isso, é necessário que se retire de dentro do comando de controle da estrutura de repetição alguns dos elementos que predeterminam a quantidade de iterações a serem realizadas. Em termos de algoritmos, seria algo semelhante ao que é trazido na imagem 25.

CONTADOR <- 1

PARA CONTADOR ATÉ 100 FAÇA

ESCREVA (“ITERAÇÃO “, CONTADOR);

CONTADOR <- CONTADOR + 1

FIMPARA;

Imagem 25: Exemplo de estrutura de repetição contada. | Fonte: O autor.

Com as alterações feitas no exemplo da imagem 24 para a obtenção do exemplo da imagem 25, houve aumento na quantidade de linhas necessárias para gerar o trecho de algoritmo com a mesma funcionalidade do anterior, mas retirando de dentro do comando da estrutura o controle total do laço de repetição.

Essa forma de se construir uma estrutura de repetição com base na palavra reservada “PARA” é muito comum no meio profissional, se aproximando do uso das demais palavras reservadas estudadas nesta aula, mas a escolha entre o uso de cada opção de comando depende do que é preciso fazer em cada problema e da forma como cada desenvolvedor aplica sua lógica na elaboração de soluções.

Estruturas de repetição são excelentes recursos para o desenvolvimento de algoritmos e é importante observar que o tipo de laço contado representado nesta aula pela palavra reservada “PARA” é uma opção que possui sintaxe que permite que todos os parâmetros colocados definam exatamente a quantidade de iterações a serem realizadas, mas é possível ajustar esta opção de laço omitindo partes dos parâmetros e utilizando-os fora do comando “PARA” de forma a poder controlar a quantidade de iterações a partir dos processos ocorridos durante as iterações.

O uso dos comandos “ENQUANTO...FAÇA” ou “REPITA...ATÉ” possui a particularidade de terem a diferença da condição colocada no início do laço ou no final, variando o controle realizado e tendo assim, a possibilidade de ocorrerem ou não iterações no laço.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Estruturas de Controle
- Estruturas de Repetição Condicional
- Estruturas de Repetição Contada

Para complementar seus estudos, assista à videoaula a seguir: