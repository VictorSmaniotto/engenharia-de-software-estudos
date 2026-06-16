---
title: "aula-09"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-09.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 09 - Aninhamento de Estruturas

Sumário

## Aninhamento de Estruturas de Controle

Aos poucos, à medida que os estudos vão avançando na disciplina e novos conceitos vão sendo conhecidos, é normal que se possam ter pensamentos sobre como se podem interligar conceitos aprendidos até então e como integrar estes conceitos pode contribuir para um melhor aprendizado.

Nesta disciplina, os conceitos são todos complementares e a cada novo conceito, este pode ser integrado aos demais, pois é comum em algoritmos maiores que praticamente todas as estruturas e palavras reservadas estudadas até então sejam utilizadas.

Assim, é mais fácil compreender o todo em relação ao aprendizado da disciplina, e também facilita o aprendizado dos conceitos separados, pois são frequentemente reaplicados em novas aulas deste material.

Imagem ilustrativa.

[Disponível aqui](https://elements.envato.com/pt-br/engenheiros-de-software-qualificados-discutindo-JPL9R4K)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a09-img1.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/img-icon-quadrado-2.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/img-icon-bola-2.svg)

É importante utilizar o espaço desta aula para uma complementação do que foi estudado até o momento de forma a mostrar de que maneira os conceitos estudados podem contribuir como desenvolvimento de algoritmos.

Por meio de alguns exemplos comentados e alguns apontamentos pertinentes, a ideia é analisar as possibilidades de criação de algoritmos a partir do que já se sabe e preparar o terreno para a adição de novos conceitos nas aulas seguintes.

Como estas estruturas possuem uma maior complexidade lógica, será usado um artifício bastante útil em teste de algoritmos chamado de teste de mesa, em que se utilizam amostras de dados escolhidas aleatoriamente ou de forma tendenciosa para simular a execução de algoritmos e buscar possíveis falhas se houver.

Para cada exemplo desta aula e em outras de aulas posteriores vamos demonstrar a lógica e funcionalidade de algoritmos que possam ser mais complexos e necessitarem de esclarecimento adicional mais prático.

Os testes de mesa são utilizados por autores como Manzano (1997) como meios para exibir dados a serem utilizados em simulações de algoritmos e também para conter os dados obtidos com o processamento dos dados escolhidos para testes.

## Aninhamento de Estruturas de Decisão

O uso de estruturas condicionais é bastante comum, pois, como já dito, permitem que sejam tomadas decisões durante a execução de um algoritmo de forma automatizada, pelo próprio algoritmo.

Seu uso é simples em sua estrutura, mas a elaboração de expressões pode ser complexa e necessitar de boa análise lógica para prever os possíveis resultados e erros na formulação da expressão de controle.

Também é importante ter bem clara a composição de estruturas de decisão de forma que uma estrutura posta dentro de outra estrutura apenas pode ser executada em caso de a estrutura na qual está inserida obtiver resultado verdadeiro em sua expressão condicional.

Observe o exemplo a seguir contido na imagem 26 para compreender melhor como se podem organizar as alternativas de execução de um algoritmo por meio de estruturas aninhadas de decisão.

SE (A >= B) ENTÃO

SE (A >= C) ENTÃO

ESCREVA (“A PODE SER O MAIOR VALOR”);

SENÃO SE (C >= A) ENTÃO

ESCREVA (“C PODE SER O MAIOR VALOR”);

SENÃO

SE (B >= C) ENTÃO

ESCREVA (“B PODE SER O MAIOR VALOR”);

SENÃO

ESCREVA (“C PODE SER O MAIOR VALOR”);

ESCREVA (“DEVE HAVER NÚMEROS IGUAIS”);

FIMSE.

Imagem 26: Exemplo de estrutura de repetição contada.

### TESTE DE MESA

| **A** | **B** | **C** | **RESULTADO** |
| --- | --- | --- | --- |
| 1 | 2 | 3 | C PODE SER O MAIOR VALOR |
| 2 | 3 | 1 | B PODE SER O MAIOR VALOR |
| 3 | 2 | 1 | A PODE SER O MAIOR VALOR |
| 1 | 1 | 1 | DEVE HAVER NÚMEROS IGUAIS |

Fonte: O autor.

Neste exemplo da imagem 26 é exibido um trecho de algoritmo contendo um encadeamento de estruturas condicionais para verificar três valores e determinar qual o maior em caso de todos serem diferentes e uma análise profunda ser possível, ou indicar que deve haver números iguais, dificultando a avaliação do maior.

A estrutura de decisão poderia ser mais completa e avaliar mais casos, pois é importante ter a noção de que para três variáveis, é possível uma série de combinações de comparações que podem ser feitas entre estes valores, resultando em diferentes cenários.

Importante é compreender a lógica do encadeamento de estruturas de forma que algumas comparações são realizadas apenas se a anterior for verdadeira na primeira estrutura encadeada.

A segunda estrutura encadeada depende da primeira resultar falsa para ser avaliada, e assim, a forma como se estruturam encadeamentos de estruturas devem ser bem planejadas para evitar problemas em sua execução.

## Aninhamento de Estruturas de Repetição

Continuando com os estudos de integração entre conceitos vistos nas aulas anteriores, é o momento de avaliar melhor o uso das estruturas de repetição com a intenção de agrupar estruturas de repetição de forma aninhada para que se possam realizar duas ou mais iterações paralelamente.

Este tipo de recurso é importante em situações como no caso de ser necessário realizar leituras ou atualizações de dados em estruturas multidimensionais que serão estudadas mais adiante, mas também em casos em que sejam necessários contadores ocorrendo de forma complementar como em ponteiros de relógios, contadores do tipo hodômetro, etc.

Este tipo de estrutura pode ser confuso inicialmente, mas depois de compreendido, é um recurso útil e muito utilizado nas estruturas multidimensionais pela facilidade de sua implementação e funcionamento preciso.

PARA I DE 0 ATÉ 9 PASSO 1 FAÇA

PARA J DE 0 ATÉ 0 PASSO 1 FAÇA

PARA K DE 0 ATÉ 9 PASSO 1 FAÇA

ESCREVA (I, J, K);

FIMPARA;

FIMPARA;

FIMPARA;

Imagem 27: Exemplo de estrutura de repetição aninhada. | Fonte: autor.

Neste exemplo da imagem 27 é implementado um trecho de algoritmo para simular o funcionamento de um hodômetro com três dígitos, e para isto, são necessárias três variáveis para cada um dos três dígitos utilizados neste algoritmo.

Cada dígito do hodômetro deve ser trocado em um momento específico que é quando o dígito a sua direita completar um ciclo completo de 0 a 9, exceto pelo primeiro dígito da direita que representa a unidade a partir da qual os demais dígitos sucessivamente se baseiam para suas trocas de valores.

Com três dígitos, o resultado do comando “ESCREVA” será a exibição dos dígitos de centena, dezena e unidade de 000 a 999, sequencialmente, como ocorre em contadores manuais ou digitais.

O aninhamento ou encadeamento de estruturas de controle de mesmo tipo é bastante utilizado na elaboração de algoritmos e permite que algoritmos com necessidades mais complexas possam ser elaborados.

Estruturas de dados maiores que variáveis, por exemplo, necessitam de recursos mais complexos para sua manipulação, assim como condições que são avaliadas em sequência podem ser encadeadas de forma a se complementarem, e assim, permitir situações nas quais uma avaliação é realizada apenas dependendo do resultado obtido em uma condição anterior realizada necessariamente primeiro.

Estruturas de repetição encadeadas permitem que dois contadores ou mais estejam trabalhando em conjunto como nos números de um hodômetro ou ponteiros de um relógio, e assim, cada vez mais funcionalidades são obtidas pela combinação de estruturas de controle.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg)

## Estruturas de Repetição em Estruturas de Decisão

Seguindo em frente com os estudos mais avançados no uso de estruturas de controle, é possível combinar estruturas diferentes de forma que possam ser integradas e realizem processamento mais complexo.

Estruturas de repetição podem ser inseridas dentro de estruturas de decisão de forma que determinado laço de repetição seja acionado apenas se determinada condição for satisfeita, para que a partir deste desvio de fluxo, a expressão de controle do laço seja avaliada para que sejam ou não iniciadas as iterações.

VALOR <-10;

SE (VALOR > 0) ENTÃO

PARA I DE 1 ATÉ VALOR PASSO 1 FAÇA

ESCREVA (I);

FIMPARA;

FIMSE;

Imagem 28: Exemplo de estrutura de repetição em estrutura de decisão. | Fonte: O autor.

No exemplo trazido na imagem 28, é colocado um laço de repetição que exibirá valores entre 1 e o número contido na variável “VALOR”, inicialmente atribuído com 10, mas isto só ocorre em função da verificação da condição do comando “SE” resultar verdadeiro, pois “VALOR” possui número maior que 0.

## Estruturas de Decisão em Estruturas de Repetição

Por último e não menos importante, existe outra forma de se combinar estruturas de controle de fluxo em algoritmos na qual estruturas de decisão podem ser inseridas em estruturas de repetição para que possam ser avaliadas novamente a cada iteração de um laço de repetição.

Um exemplo seria no caso do preenchimento de uma estrutura mais complexa de dados que utilizaria um laço de repetição para percorrer todos os espaços para armazenamento, mas os dados destes seriam atualizados apenas em caso de uma expressão avaliada a cada iteração resultar verdadeiro, por exemplo.

VALOR <- 10;

PARA I DE 1 ATÉ VALOR PASSO 1 FAÇA

SE (I=5) ENTÃO

I <- VALOR;

FIMSE;

FIMPARA;

Imagem 29: Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: autor.

Neste outro exemplo contido agora na imagem 29, é inicializada uma variável “VALOR” com 10 para que possa servir de base para um laço de repetição que inicialmente está programado para realizar 10 iterações com uma variável contadora “I” variando de 1 a 10 pela definição do comando “PARA”.

Existe internamente ao laço de repetição, uma estrutura condicional que verifica a cada iteração o conteúdo da variável “VALOR”, e caso seja igual a 5, força o conteúdo da variável “VALOR” ser ajustado para 10, encerrando as iterações na próxima verificação da condição de parada das repetições.

O chamado aninhamento de estruturas de controle é um recurso muito útil e acrescenta muitos recursos no desenvolvimento de algoritmos, mas também traz um aumento na complexidade de algoritmos que pode confundir iniciantes.

É importante praticar o desenvolvimento de pequenos algoritmos contendo estruturas de controle variadas para compreender a mecânica dos aninhamentos e como uma estrutura possui influência sobre a outra, além de compreender melhor os motivos necessários para aninhar estruturas e como definir quais tipos são adequados a cada situação.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Aninhamento de Estruturas de Controle
- Aninhamento de Estruturas de Decisão
- Aninhamento de Estruturas de Repetição
- Estruturas de Repetição em Estruturas de Decisão
- Estruturas de Decisão em Estruturas de Repetição

Para complementar seus estudos, assista à videoaula a seguir: