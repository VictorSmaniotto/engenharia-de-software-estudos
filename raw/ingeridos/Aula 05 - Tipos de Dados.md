---
title: "Aula 05 - Tipos de Dados"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-05.html"
author:
published:
created: 2026-05-28
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 05 - Tipos de Dados

Sumário

## Noções de Dados e Tipos Básicos

A base da tecnologia da informação são os dados. Sejam eles dos tipos mais simples como números ou texto, ou mais complexos como estruturas heterogêneas de dados, imagens, sons, etc., todos são formados por bits e seu processo de armazenamento é semelhante em qualquer dos tipos.

Em algoritmos os dados devem ser definidos logo no momento da declaração de uma estrutura de dados, e geralmente, logo no início do algoritmo, antes do início da escrita das instruções que servirão para manipular estes dados.

Os tipos básicos de dados para manipulação são os utilizados para armazenamento temporário e manipulação de valores numéricos inteiros ou decimais, caracteres simples que englobam símbolos gerais do teclado como letras, números, e demais símbolos, e por último, um quarto tipo se refere a valores verdadeiro e falso apenas chamado lógico.

Estes tipos podem ser usados livremente na implementação e algoritmos, mas precisam estar associados a estruturas de dados de forma a definirem quais tipos de dados são aceitos por cada estrutura de dado declarada.

## Estruturas Básicas de Dados (variáveis)

As estruturas de dados podem ser simples espaços em memória para armazenamento de um único dado declarado com algum dos tipos básicos citados e servem como armazenamento temporário em memória para uso durante a execução de um algoritmo.

Esse tipo de estrutura de dado é chamado de variável em função da volatilidade alta dos dados inseridos nestas, em função da possibilidade de troca dos dados inseridos e da perda dos mesmos ao final da execução do algoritmo.

As variáveis devem ter seus tipos definidos em suas declarações por padrão, mas não há impedimentos de alguém optar por não definir tipos e apenas no momento em que uma variável declarada sem tipo definido receber um dado, este definirá qual o tipo associado à variável, mas isso reduz a previsibilidade do algoritmo e aumenta as chances da ocorrência de erros.

Em geral, a sintaxe para declaração de variáveis, segundo Forbellone (2005), define que a declaração se inicia pelo tipo de dado a ser associado à variável, seguido do símbolo “:” que age como separador, e em seguida, o nome (identificador) que será atribuído à variável, finalizando com um símbolo “;” a instrução. Observe os exemplos da imagem 10.

INTEIRO: IDADE

REAL: PESO, ALTURA

CARACTERE: LETRA

LÓGICO: TESTE

Imagem 10: Exemplos de declaração de variáveis. | Fonte: O autor.

Nos exemplos da imagem 15, são declaradas variáveis de tipos distintos para que sejam conhecidos todos os tipos básicos, sendo “INTEIRO” para números sem casas decimais, e “REAL” para números que aceitam casas decimais. O tipo “CARACTERE” é utilizado para caracteres diversos, mas também pode ser utilizado para texto em geral contendo uma série de caracteres de qualquer quantidade. Por fim, o tipo “LÓGICO” é usado para variáveis que possam aceitar apenas os estados lógicos verdadeiro ou falso.

Alguns detalhes importantes para que se compreenda melhor a sintaxe de algoritmos baseados no padrão adotado por Forbellone (2005), ao final da maior parte das instruções, é utilizado o símbolo “;” para indicar que a instrução encerra no ponto em que houver este símbolo, e assim, mesmo que uma instrução seja dividida em mais de uma linha, as quebras de linhas não simbolizam final de instrução, mas não será utilizado este padrão neste material para maior facilidade de compreensão.

Outro símbolo importante utilizado no exemplo da imagem 15 é “,” que serve como separador para o caso de duas ou mais variáveis serem declaradas com um mesmo tipo, economizando assim, digitação e linhas de código.

As variáveis funcionam como depósitos de dados que podem ser manipulados durante a execução e algoritmos e devem ser bem compreendidas para que seu uso constante não represente um problema. As constantes complementam as variáveis como recurso para armazenamento de dados não variáveis durante a execução de algoritmos.

Acesse o link:[Disponível aqui](https://www.embarcados.com.br/variaveis-e-constantes/)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Atribuição de Dados

Após a declaração de variáveis ou outras estruturas de dados, estas ficam disponíveis para o algoritmo que pode inserir e alterar dados nestas livremente, lembrando que estas são estruturas temporárias, e ao final da execução do algoritmo, os dados são perdidos com a liberação da memória utilizada pelo algoritmo.

Para que dados sejam adicionados a variáveis e outras estruturas, um dos meios mais utilizados é a chamada atribuição de dados que utiliza o símbolo “<-“ para que o dado ou resultado de uma expressão que esteja à direita do símbolo seja adicionado à estrutura de dado. Observe os exemplos da imagem 11.

IDADE <- 20;

PESO <- 50.5;

NOME <- “RONIE”;

MEDIA <- (VALOR1 + VALOR2) / 2;

Imagem 11: Exemplos de atribuição de dados a variáveis. | Fonte: O autor.

Pelos exemplos da imagem 11, é possível compreender a forma como se realizam atribuições simples de valores a variáveis como nos três primeiros exemplos que atribuem um valor inteiro, um decimal e uma *string* (como também pode ser chamada uma sequência de caracteres quaisquer), respectivamente.

O último exemplo da imagem 16 traz uma expressão que tem seu resultado atribuído à variável “MEDIA”, lembrando que o cálculo de expressões é realizado antes de a atribuição ser realizada.

O uso de estruturas de dados como variáveis é fundamental para o desenvolvimento de algoritmos e saber manipular seus dados de forma adequada é importante. Uma prática que auxilia a desenvolver algoritmos seguros é a do uso da atribuição para realizar inicializações de variáveis antes de seu primeiro uso, pois assim, valores indesejados contidos na área de memória alocada para variáveis não correm o risco de serem utilizados.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

## Exemplos de Algoritmos com Variáveis

Tendo então conhecimento dos elementos essenciais de um algoritmo em relação à aquisição e tratamento de dados, é interessante conhecer a estrutura básica de um algoritmo e assim, já estar habilitado a formular pequenos algoritmos, mesmo que com funcionalidades mínimas ainda.

Os autores costumam divergir sobre a forma como constroem algoritmos e em função disto, é mais complexa a citação de um ou outro autor especificamente, mas para este material, foram unidos elementos utilizados por três autores distintos sendo estes Forbellone (2005), Manzano (1997) e Ascencio (2012) para que se possam aproveitar aspectos positivos de cada um deles e compor um estudo bem completo da elaboração de algoritmos.

Para este material, a estrutura básica para algoritmos seguirá alguns padrões como, por exemplo, o uso de letras maiúsculas, apenas para maior destaque visual no texto, sintaxe seguindo o padrão utilizado por Ascencio (2012) que utiliza pequena quantidade de símbolos na construção das instruções que possuem o mesmo significado das sintaxes de outros autores que escrevem seus algoritmos de forma um pouco diferente.

Observe o exemplo da imagem 12 para conhecer a estrutura básica de elaboração de algoritmos neste material, observando as palavras reservadas utilizadas em instruções e os elementos que complementam estas palavras reservadas em muitos casos, chamados de parâmetros para as palavras reservadas.

INÍCIO

DECLARE

INTEIRO A, B, C;

A <- 10;

B <- A \* 2;

C <- A \* B;

FIM.

Imagem 12: Exemplos de atribuição de dados a variáveis. | Fonte: O autor.

Neste exemplo de algoritmo completo da imagem 12, observa-se a estrutura básica de escrita de algoritmos usada nesse material onde a palavra reservada INÍCIO, como foi utilizado em exemplos anteriores, é a primeira instrução.

Logo em seguida, a palavra reservada DECLARE indica a declaração de variáveis e outras estruturas de dados a partir deste ponto, e neste exemplo, são declaradas três variáveis A, B e C do tipo inteiro para uso no processamento do algoritmo.

Logo em seguida da declaração, ocorre uma atribuição do valor inteiro 10 para a variável A, onde se utiliza o símbolo padrão “<-“ para indicar a atribuição, e o símbolo “;” para encerrar a instrução como já comentado anteriormente.

Em seguida, em uma segunda instrução de atribuição, o valor de A, 10, é multiplicado por 2 resultando em um valor 20 a ser atribuído à variável B, e por fim, em uma última instrução de atribuição, os valores 10 da variável A e 20 da variável B são multiplicados para que o valor resultante 200 seja armazenado em C.

A elaboração de algoritmos parece simples inicialmente, mas tende a tornar-se mais complexa à medida que são incluídas novas estruturas e palavras reservadas com funcionalidades que necessitam de maior esforço lógico para a elaboração de soluções complexas.

  <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Noções de Dados e Tipos Básicos
- Estruturas Básicas de Dados (variáveis)
- Atribuição de Dados
- Exemplos de Algoritmos com Variáveis

Para complementar seus estudos, assista à videoaula a seguir: