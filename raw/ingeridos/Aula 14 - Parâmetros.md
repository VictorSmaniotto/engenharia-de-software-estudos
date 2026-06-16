---
title: "Aula 14 - Parâmetros"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-14.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 14 - Parâmetros

Sumário[1\. Sub-Rotinas: Passagem de Parâmetros](#topico-01)[

2\. Passagem de Parâmetros por Valor

](#topico-02)[

3\. Passagem de Parâmetros por Referência

](#topico-03)

## Sub-Rotinas: Passagem de Parâmetros

Continuando os estudos iniciados na aula anterior, as sub-rotinas, sejam elas procedimentos ou funções, já se mostraram recursos extremamente úteis para tornar algoritmos mais bem estruturados e mais facilmente reutilizáveis.

O uso das sub-rotinas até então depende do escopo das estruturas de dados para que possam ser funcionais, e dependendo do escopo destas estruturas, poderia inviabilizar o desenvolvimento de parte dos algoritmos de forma estruturada em sub-rotinas.

Um exemplo de caso em que o escopo pode gerar problemas, é no caso de um algoritmo possuir duas ou mais sub-rotinas, além do algoritmo principal, e em algum momento, uma sub-rotina necessitar de dados que estavam armazenados em estruturas de dados contidos em outra sub-rotina, e assim, estas seriam de escopo local.

Além disso, existe ainda o problema de que estruturas de dados locais em uma sub-rotina deixam de ter validade e perdem seus dados quando a sub-rotina for encerrada, e a execução retorna ao ponto de onde foi chamada. Isto gera um problema, pois não é possível o uso de dados processados em estruturas de dados locais de uma sub-rotina em outra a princípio, mas existe uma forma de evitar a perda de dados de estruturas locais com o encerramento de uma sub-rotina.

É possível que dados sejam passados de uma sub-rotina a outra por meio de parâmetros que servem como ligação de dados entre sub-rotinas, ou entre sub-rotinas e o algoritmo principal.

## Passagem de Parâmetros por Valor

A passagem de parâmetros pode ocorrer de duas formas, sendo a primeira delas chamada de passagem por valor em que dados são passados diretamente de um ponto do código que chama uma sub-rotina para dentro da mesma, podendo ser utilizado livremente pelos processos da sub-rotina.

A passagem de dados diretamente de uma parte de um algoritmo para dentro de uma sub-rotina representa que um valor específico ou uma cópia do conteúdo contido em uma estrutura de dados é enviado para uma sub-rotina, e isto não afeta o valor original na origem onde foi gerada a chamada da sub-rotina.

Assim, qualquer processamento realizado sobre o valor recebido como parâmetro por uma sub-rotina se mantém apenas durante a execução da sub-rotina, e estas alterações são perdidas, a menos que a sub-rotina seja uma função e o dado processado seja retornado ao ponto do algoritmo que chamou a sub-rotina.

No caso de procedimentos, como não há retorno de dados, parâmetros passados por valor servem apenas como dados simples para auxiliar nos processamentos implementados no procedimento.

No caso de funções, estas podem ser implementadas com o intuito de que os processamentos internos sejam organizados para realizar alterações necessárias em dados recebidos como parâmetros para que os retornos possam obter novos dados relevantes para a continuidade da execução de um algoritmo sem alterar dados contidos em fontes originais usadas para preenchimento dos dados utilizados como argumentos para os parâmetros permitidos pela função.

PROCEDIMENTO CALCULA ( INTEIRO: V1, V2, V3)

DECLARE

INTEIRO: SOMA;

SOMA <- V1 + V2 + V3;

ESCREVA (“RESULTADO = “, SOMA);

FIM;

Imagem 42: Exemplo de passagem de parâmetro por valor. | Fonte: O autor.

No exemplo trazido na imagem 42, temos uma função para cálculo da soma de três valores. Dentro desta função, alguns detalhes devem ser observados como a declaração de três parâmetros que funcionarão como variáveis a serem utilizadas pela função “CALCULA” do tipo inteiro e chamadas de “V1”, “V2”, “V3”.

Estes parâmetros são a forma mais adequada de passagem de dados entre uma função e algum ponto do algoritmo que possa chamar a execução desta função para a realização de processos necessários.

Assim, estes parâmetros servirão como receptores de dados vindos de fora da sub-rotina, mas é importante observar que neste tipo de passagem de parâmetros por valor, apenas uma cópia dos dados é utilizada como argumento para cada parâmetro, e os dados originais permanecerão inalterados durante a execução da sub-rotina.

Parâmetros representam a comunicação entre partes de um algoritmo divididas em sub-rotinas. Esta comunicação é muito importante para que o fluxo de dados que transitam entre as sub-rotinas permita que algoritmos possam dividir o processamento de seus dados em partes.

Situações como cálculos a serem realizados podem estar em sub-rotinas diferentes num algoritmo em relação à obtenção dos dados, e com a passagem de parâmetros por valor, estes dados podem ser enviados a uma sub-rotina que efetue os cálculos necessários e exiba resultados, por exemplo.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

## Passagem de Parâmetros por Referência

Outro tipo de parâmetro que pode ser utilizado em sub-rotinas possui uma forma de utilização diferente e acaba sendo não uma alternativa à passagem de valor, mas sim, utilizado para outro tipo de finalidade. Na passagem de parâmetro por referência, os dados em si não são passados de uma parte do algoritmo para o interior de uma sub-rotina como cópia do valor original.

Nesse tipo de passagem de parâmetros, os dados em si se mantêm nas estruturas de origem no algoritmo chamador, e referências a estas estruturas são passadas para que possam ser diretamente manipuladas pela sub-rotina e todos os processamentos realizados afetam diretamente os dados contidos em estruturas de dados externas à sub-rotina como se fossem estruturas de dados locais.

O uso deste recurso é importante, pois pode auxiliar no sentido de que dados não precisem ser replicados para serem utilizados em sub-rotinas, e ainda economiza recurso de *hardware* com um menor uso de memória e processamento para seu gerenciamento, ponto relevante no desenvolvimento de *software* para dispositivos com menor poder de processamento e memória.

Os parâmetros se referem a dados esperados por sub-rotinas para seu processamento, mas existe um termo chamado argumento que se confunde com o termo parâmetro. Na verdade, parâmetro representa o valor esperado pela sub-rotina e argumento é o dado passado como parâmetro para a sub-rotina.

Acesse o link:[Disponível aqui](https://docs.microsoft.com/pt-br/dotnet/visual-basic/programming-guide/language-features/procedures/differences-between-parameters-and-arguments)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

PROCEDIMENTO CALCULA (INTEIRO: V1, V2, V3, VAR INTEIRO: SOMA)

SOMA <- V1 + V2 + V3;

FIM;

Imagem 43: Exemplo de passagem de parâmetro por referência.| Fonte: O autor.

Neste exemplo contido na imagem 43, a proposta da sub-rotina é a mesma do exemplo apresentado na imagem 42 de somar três valores, mas a construção da sub-rotina foi feita de forma diferente, utilizando o conceito da passagem de parâmetros por referência.

A distinção em termos de declaração da sub-rotina é sutil, mas faz muita diferença na prática, pois a adição da palavra reservada “VAR” no parâmetro “SOMA” faz com que este dado que será enviado como argumento pelo trecho do algoritmo que chame esta sub-rotina.

Assim, ao invés de uma cópia do dado contido na variável ser passada como cópia no argumento enviado pelo algoritmo à sub-rotina, uma referência à própria origem do dado é passada como argumento para o parâmetro, e assim, toda modificação que for realizada no valor do parâmetro, na verdade altera o dado original do algoritmo que chamou a sub-rotina.

O uso de sub-rotinas é bastante comum e importante no desenvolvimento de algoritmos pelas suas diversas características. De forma complementar aos estudos e prática de elaboração de algoritmos modulares utilizando sub-rotinas, é essencial que seja conhecido e praticado o uso da passagem de parâmetros.

Cada situação distinta poderia necessitar de parâmetros que fossem ou não utilizados para passagem de dados entre partes de um algoritmo, e se o melhor mecanismo para cada caso é a passagem por valor ou por referência.

Buscar sempre elaborar algoritmos de forma modular é uma excelente prática e permite além da prática dos conceitos estudados nesta unidade, o aprendizado de importante técnica de reduzir problemas maiores em problemas de menor complexidade, facilitando o desenvolvimento de soluções e a maior modularização dos algoritmos de forma natural.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Sub-Rotinas: Passagem de Parâmetros
- Passagem de Parâmetros por Valor
- Passagem de Parâmetros por Referência

Para complementar seus estudos, assista à videoaula a seguir: