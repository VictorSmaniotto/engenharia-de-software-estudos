---
title: Aula 04 - Programação Estruturada - Linguagem C
source: https://ead.unimar.br/aulas/linguagens-de-programacao/aula-04.html
author:
published:
created: 2026-05-11
description:
tags:
---
Conhecer a base de uma linguagem de programação é essencial para que se possa implementar software para a solução de problemas diversos, mas apenas conhecer a linguagem não é suficiente para que se possa considerar o desenvolvedor um bom programador, pois saber avaliar problemas e sua complexidade, elaborar algoritmos eficientes, ser capaz de detectar falhas ou melhorias possíveis, testar a solução pensada de forma a garantir o máximo de funcionalidade possível a ser entregue e ser capaz de implementar a solução em uma linguagem conhecida, ou escolher a mais adequada dentre as conhecidas são atribuições de um profissional dito programador ou desenvolvedor.

O conhecimento dos diferentes paradigmas ajuda inclusive a escolher as linguagens mais interessantes para se conhecer e se necessário, aprender para que se tenha conhecimento do que se pode desenvolver com determinada linguagem, mas um ponto a ser levado em consideração é que mão de obra qualificada para apenas codificar é mais barata que a necessária para se avaliar problemas e propor algoritmos que resolvam estes problemas de forma eficiente e confiável.

A linguagem C talvez seja o exemplo mais apropriado de linguagem para estudo da programação estruturada por vários motivos, sendo um deles a sua extensa lista de funcionalidades implementadas, sendo capaz de produzir código voltado para soluções de baixo a alto níveis e aumentando o leque de desenvolvimento de software a partir das suas variações C++, C# e Objective-C, por exemplo que elevaram a linguagem para desenvolvimento de software para outras áreas como da computação gráfica e desenvolvimento web.

## Linguagem C

A base da linguagem C são as sub-rotinas que representam blocos de códigos inseridos em estruturas chamadas de **funções,** que funcionam independentes entre si, necessitando que dados sejam passados entre si para que possam trabalhar os mesmos dados durante a execução do software gerado a partir delas.

Todo código em linguagem C não precisa ter várias funções, mas também não pode ser implementado sem o uso de nenhuma função, pois a execução de um software desenvolvido em linguagem C parte sempre de uma função chamada main() que inclusive não pode ter este nome utilizado em nenhuma outra função no mesmo software.

Outra característica da linguagem C é que ela é case sensitive, ou seja, trata **maiúsculas e minúsculas de formas distintas,** e como padrão, todas as palavras reservadas da linguagem devem ser digitadas em letras minúsculas.

Alguns elementos que não necessariamente estão ligados à lógica, mas são necessários à sintaxe na codificação, foram adotados por muitas linguagens de programação que se baseiam em C, como a linguagem Java, por exemplo.

Os caracteres ponto e vírgula, chaves, parênteses e colchetes são delimitadores de comandos ou outros elementos que serão citados logo na sequência e que são fundamentais para que cada instrução possa ser bem definida e completa.

As chaves são utilizadas para delimitar blocos de comandos dentro de instruções mais complexas como desvios condicionais ou laços de repetição que permitem que comandos diversos (inclusive outras estruturas semelhantes) sejam inseridos dentro de seus blocos a serem executados.

O aninhamento ou encadeamento de estruturas de controle de mesmo tipo é bastante utilizado na elaboração de algoritmos e permite que algoritmos com necessidades mais complexas possam ser elaborados. Estruturas de dados maiores que variáveis, por exemplo, necessitam de recursos mais complexos para sua manipulação, assim como condições que são avaliadas em sequência podem ser encadeadas de forma a se complementarem e, assim, permitires situações em que uma avaliação é realizada apenas dependendo do resultado obtido em uma condição anterior realizada necessariamente primeiro. Estruturas de repetição encadeadas permitem que dois contadores ou mais estejam trabalhando em conjunto como nos números de um hodômetro ou ponteiros de um relógio, e assim, cada vez mais funcionalidades são obtidas pela combinação de estruturas de controle.

![início da abordagem prática](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-abordagem-center.svg)

Veja a imagem a seguir:

int avaliação(int idade, char experiencia) {

if (idade >= 18) {

if (experiencia = “S”) {

printf (“Candidato aceito para entrevista\\n”);

return (1);

} else {

printf (“Candidato não atendeu os requisitos\\n”);

return (0);

}

} else {

printf (“Candidato não atendeu os requisitos\\n”);

return (0);

}

}

Fonte: autor.

Observando o exemplo acima, temos uma função chamada **avaliação** (apenas letras sem acento são permitidas em identificadores) contendo dois parâmetros que funcionam como requisitos para a funcionalidade da função.

Assim, temos que os **parênteses**, além de seu uso em expressões matemáticas, serve para **delimitar parâmetros** que representam dados passados de uma função a outra ou para atender à sintaxe de comandos – como **if** – utilizados no exemplo.

Os comandos if contêm expressões lógicas baseadas em operadores lógicos, e realizam desvios da execução do software de acordo com os valores resultantes da condição definida, assim como outra palavra reservada importante no exemplo é else que representa a contrapartida de cada comando if de desvio condicional utilizado.

O espaçamento em níveis chamado de **endentação** (ou indentação também), que não é obrigatório nesta linguagem, auxilia na legibilidade do código e para compreender as estruturas de decisão if e else, e como estão estruturados dentro da função avaliacao().

Para se conhecer uma linguagem de programação como C, é preciso se familiarizar com sua semântica, que representa a forma como um código deve ser estruturado e a variedade de diferentes estruturas sintáticas que são as regras de construção de instruções a partir de comandos e funções da linguagem. Também é muito importante ler códigos prontos e compreendê-los, mas é preciso também executá-los, modifica-los e depois tentar criar suas próprias versões de códigos e poder sentir segurança para atuar profissionalmente com uma linguagem qualquer.

![início da abordagem prática](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-abordagem-center.svg)

O trecho de código da imagem anterior não pode ser compilado da forma como está, pois existe um complemento necessário semântico composto de outros comandos e elementos para que o compilador possa gerar um software executável, e o exemplo de estrutura básica em linguagem C da imagem a seguir pode ser observado.

#include <stdio.h>

int main () {

int idade;

char experiencia;

int vaga = 0;

while (vaga <= 10) {

printf (“Digite sua idade: );

scanf (“%d”, &idade);

printf (“Digite sua experiência: );

scanf (“%d”, &experiencia);

vaga = vaga + avaliacao (idade, experiencia);

}

return (0);

}

Fonte: autor.

Neste exemplo, o restante do código necessário para que se possa gerar um software é exposto, sendo que ambos os trechos das imagens anteriores devem estar posicionados em um mesmo arquivo de texto salvo com o nome desejado, seguido da extensão **.C** indicativa de códigos desta linguagem.

Uma estrutura de repetição representada pelo comando **while** que se baseia em uma condição indicada dentro dos parênteses como parâmetro para controlar a quantidade de repetições a serem realizadas tem como base uma suposta ideia de que existe um processo de chamada de até dez pessoas para a realização de entrevista para possível contratação, por exemplo.

Dentro da função **main()** são obtidos os dados necessários para processamento na função avaliacao() através das funções printf() e scanf() que estão disponíveis numa biblioteca adicionada pela primeira instrução do código que inclui a stdio.h, e assim disponibiliza estas duas funções e muitas outras criadas para esta finalidade.

A codificação em linguagem C pode ser bastante complexa devido ao grande detalhamento dos processos que podem ser implementados, e linguagens mais modernas simplificam esse desenvolvimento, que reduz o trabalho de codificação, mas reduz também a possibilidade de manipulação de como deve ser realizado o processo.

Existem estruturas geradas em linguagem C que não existem em várias outras linguagens tais como Java, como os chamados ponteiros que servem como indicativos de outra estrutura de dados em memória e não armazenam dados em si, sendo útil em estruturas de dados mais complexas que variáveis principalmente.

void trocaValores (int a, int b) {

int aux;

aux = a;

a = b;

b = aux;

}

void trocaValores (int \*a, int \*b) {

int aux;

aux = \*a;

\*a = \*b;

\*b = aux;

}

Fonte: autor.

Nestes exemplos, temos duas variações de uma mesma função **trocaValores(),** que recebe dois parâmetros de formas distintas em cada exemplo. No primeiro, recebe uma cópia dos valores originais recebidos e alterações sofridas pelos valores contidos nas variáveis a e b não afetam as variáveis de origem dos valores, pois dentro de uma função, o chamado **escopo** de uma variável faz com que variáveis declaradas dentro de uma função, sejam ativas apenas durante a execução da função, tendo sido criada no momento da execução da função, e tendo o espaço ocupado pela mesma na memória liberada assim que a função é encerrada.

No segundo exemplo da imagem acima, os parâmetros são, na verdade, ponteiros que são direcionados nas posições de memória ocupadas pelas variáveis de origem indicadas como parâmetros, e quaisquer alterações sofridas pelos ponteiros da função afetam e alteram diretamente os valores das variáveis fora da função ligadas aos parâmetros da função, sendo então a maneira correta de conseguir alterar mais de um valor de uma variável em uma função, pois usando apenas parâmetros e retornos de função, a linguagem C, assim como várias outras, tem por padrão o retorno de apenas um valor simples.

Fonte: Freepik.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a04-img01.jpg)

Outro tipo importante de estrutura de dados da linguagem C são os **vetores e matrizes**, estruturas de dados homogêneas para conjuntos de dados, sendo vetor para listas com uma dimensão apenas, e matrizes para duas ou mais dimensões, lembrando que existem autores que utilizam apenas o temo matriz para qualquer quantidade de dimensões.

A imagem a seguir mostra exemplos de vetores e matrizes com as indicações de índices para identificação de cada célula das estruturas, observando que a numeração inicia em zero por convenção da linguagem e as referências são indicadas entre colchetes.

| **  0  ** | **  1  ** | **  2  ** | **  3  ** | **  4  ** | **  5  ** | **  6  ** | **  7  ** | **  8  ** | **  9  ** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |  |  |

**int lista\[10\];**

| **0** | **1** | **2** | **3** | **4** | **5** | **6** | **7** | **8** | **9** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **1** |  |  |  |  |  |  |  |  |  |
| **2** |  |  |  |  |  |  |  |  |  |
| **3** |  |  |  |  |  |  |  |  |  |

**char dados\[3\]\[9\];**

Fonte: autor.

Na imagem, é apresentada um ilustração de um vetor declarado com o nome lista para 10 elementos do tipo inteiro, e depois, é ilustrada uma matriz declarada com o nome dados com 3 linhas e 9 colunas, totalizando uma possibilidade de armazenamento de 27 caracteres pelo tipo de dado char utilizado na declaração.

A programação estruturada trabalha com o desenvolvimento de softwares utilizando linguagens de propósito geral que normalmente e facilmente conseguem combinar estruturas de dados variadas com os demais componentes citados, sendo que as estruturas de repetição são essenciais para se trabalhar com vetores e matrizes devido a forma como funcionam ser adequada para se referenciar posições em vetores ou coordenadas de linhas e colunas em matrizes.

É comum ao observar códigos, encontrar estruturas de dados sendo referenciadas por seus nomes com símbolos como \* ou **&** juntos, e caso não conheça a capacidade de gerenciamento de memória da linguagem C, é interessante iniciar pelo conceito de ponteiros que são apontadores de endereços de memória para variáveis e outras estruturas de dados.

Fonte:[Disponível aqui](http://linguagemc.com.br/ponteiros-em-c/)

