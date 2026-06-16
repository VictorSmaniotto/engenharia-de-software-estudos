---
title: "Aula 05 - Programação Estruturada - Outras Linguagens"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-05.html"
author:
published:
created: 2026-05-11
description:
tags:
---
Sumário

Além da linguagem C, tema da aula 04, outras linguagens também são implementadas com base na programação estruturada e no paradigma imperativo como o caso da linguagem BASIC e da linguagem Pascal, além de linguagens mais populares no mercado como PHP e GO.

## Linguagem Pascal

O problema desta linguagem foi que suas evoluções acabaram sendo comercialmente fortes, como Delphi, que possui muito sistemas ativos até hoje e ainda muito confiáveis, mas mesmo Delphi não acompanhou a evolução de outras linguagens e acabou perdendo muito espaço no mercado, sendo amplamente dominado por Java, C e Python principalmente.

**program Teste;**

**var**

**a, b, potencia, i: integer;**

**begin**

**writeln ('Digite um valor inteiro para a base: );**

**readln (a);**

**potencia:= a;**

**writeln ('Digite um valor inteiro para o expoente:);**

**readln (b);**

**for i:= 1 to b-1 do**

**potencia:= potencia \* a;**

**writeln (‘Resultado da exponenciação: ‘, potencia);**

**end.**

Fonte: autor.

No exemplo da imagem acima, um código em linguagem Pascal é apresentado e sua leitura não difere muito da sintaxe da linguagem C, tendo alguns pontos de atenção a serem considerados.

Um ponto perceptível logo no início do código é que em Pascal, utiliza-se a primeira linha para nomear o código, ao invés de se incluir uma biblioteca como em C, por exemplo. Outro ponto relevante associado ao que foi citado é que os comandos de entrada e saída de dados *readln()* e *writeln()* são considerados palavras reservadas da linguagem, sendo comandos da própria implementação da linguagem.

O símbolo utilizado para atribuição de valores é:= ao invés do = utilizado em C, assim como os apóstrofos utilizados como delimitadores de texto ao invés das aspas em C, sendo igualmente importantes para a correta construção de árvores sintáticas para análise sintática de instruções.

Outro ponto importante na codificação nesta linguagem é o uso das palavras reservadas *begin* e *end* como delimitadores de blocos de comandos, tornando a legibilidade mais fácil e intuitiva.

Por fim, vale citar o uso de uma estrutura de repetição baseada na palavra reservada *for* para a criação de um laço de repetição contado onde são definidas *b-1* iterações, pois como a variável *potencia* que conterá o resultado da exponenciação é inicializada com o valor da base, uma multiplicação a menos deve ser realizada.

As variáveis funcionam como depósitos de dados que podem ser manipulados durante a execução e algoritmos e devem ser bem compreendidas para que seu uso constante não represente um problema. As constantes complementam as variáveis como recurso para armazenamento de dados não variáveis durante a execução de algoritmos. O uso de estruturas de dados como variáveis é fundamental para o desenvolvimento de algoritmos e saber manipular seus dados de forma adequada é importante. Uma prática que auxilia de se desenvolver algoritmos seguros é a do uso da atribuição para realizar inicializações de variáveis antes de seu primeiro uso, pois assim, valores indesejados contidos na área de memória alocada para variáveis não correm o risco de serem utilizados.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Observa-se que a linguagem é aparentemente mais simples em sua leitura de código, mas em relação à sintaxe e semântica, se assemelha a C, pois a construção das instruções é semelhante sofrendo poucas alterações perceptíveis, além de palavras reservadas e na simbologia utilizada.

Em Pascal também é possível incluir bibliotecas utilizando a palavra reservada *uses* que, como em outras linguagens, é utilizada semanticamente sempre no início do código, mas no caso de Pascal, logo depois da instrução que nomeia o código.

## Delphi

Em Delphi, os softwares criados se baseiam em interfaces gráficas, e a base da linguagem Pascal se mantém, mas são adicionados conceitos responsáveis por permitir que estas interfaces sejam construídas levando em consideração que o desenvolvimento de software que deva ser executado em janelas depende da mecânica de composição destas e de seus componentes disponíveis a partir das definições do sistema operacional.

Para exemplificar este tipo de aplicação implementada sobre o mesmo paradigma, mas que pode ter elementos um tanto distintos do que foi visto até o momento, observe o exemplo ilustrativo da imagem a seguir.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a05-img01.jpg) ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a05-img02.jpg)

Fonte: Bezerra (2018).

Neste exemplo, é perceptível a estrutura de uma janela típica de um sistema operacional com interface gráfica com botões, campos para entrada de dados e campos seletores de opções, e estes componentes precisam ser nomeados e funções relacionadas a eles podem ser aplicadas de forma a realizar processamento necessário.

A palavra reservada *procedure* neste exemplo age como gerenciador da janela em que os componentes necessários serão implementados e ações associadas a eles, mesmo que no processo de criação, inicialmente, os componentes sejam criados como se estivessem sendo desenhados em um software gráfico.

Cada componente criado se torna um objeto que possui propriedades associadas a ele como tamanho, core, nome, tipo, dado armazenado, etc., mas que podem ter processos codificados como se fosse em modo texto como atribuição ou modificação de valores ou cálculos matemáticos, por exemplo.

*RadioGroup1*, por exemplo, se refere ao componente que permite a seleção entre Fahrenheit ou Celcius na janela que funciona como um formulário de dados, e atributos como *ItemIndex* podem ser utilizados como for adequado ao programador, que neste caso está servindo para verificação de qual das duas opções está selecionada para cálculo da conversão de temperatura.

Dentro do bloco de comandos do primeiro comando *if* existem duas atribuições, sendo a primeira de uma expressão de cálculo da temperatura a ser atribuída à variável *conversao*. Na segunda atribuição, o valor de *conversao* é convertido em texto e adicionado como dado a ser exibido no componente *Edit2* pelo atributo *Text*.

Detalhes como a identificação de componentes e seus atributos e o uso das sub-rotinas associadas a estes são pontos divergentes em relação à linguagem Pascal original, mas a forma como se implementa o código da estrutura lógica dos processos praticamente se manteve e assim, aqueles que aprendem a linguagem pura, possuem maior facilidade de adaptação para novas versões implementadas de uma linguagem conhecida.

## Linguagem PHP

Outra opção de linguagem originalmente pensada como estruturada foi a linguagem PHP que possui um mercado muito grande para o desenvolvimento de software para sistemas web utilizando o navegador como software de interpretação de códigos.

Um ponto importante é que a linguagem PHP é associada à linguagem declarativa HTML, e juntas, realizam o processo de construção de páginas web interativas e capazes de funcionarem como sistemas criados em Delphi, por exemplo.

O HTML realiza o processo de estruturação da página em si com a inserção de elementos na página como texto, imagens, efeitos e formulários semelhantes aos criados em Delphi, sendo esta parte conhecida como Front End, ou a parte mais de interação com usuários em sistemas web.

O PHP complementa o Front End com funcionalidades como acesso a bancos de dados, processamento de dados, manipulação do que ocorre com os elementos criados em HTML e usuários, gerando funcionalidades como em sistemas desktop, processo esse associado ao termo Back End, que trabalha nos bastidores de forma mais transparente aos usuários.

**<!DOCTYPE html>**

**<html>**

**<body>**

**<h1>Exemplo HTML + PHP</h1>**

**<?php**

**$item = "Produto A";**

**$estoque = 100;**

**echo $item;**

**echo "</br>";**

**echo $estoque;**

**?>**

**</body>**

**</html>**

Fonte: autor.

Neste exemplo de código, temos as chamadas *tags* HTML responsáveis pela construção de uma página diretamente no navegador. Elas são delimitadas por sinais de < e > para caracterização das palavras reservadas e instruções completas, sendo que as instruções são estruturadas utilizando-se um comando delimitado por < e >, e depois, ao final da instrução, delimitada por < e />, indicativos de início e fim da instrução.

Internamente ao script HTML, são inseridos scripts em PHP delimitados pelos marcadores <?php e?> que separam o conteúdo PHP do restante do código HTML para impedir que o navegador interprete incorretamente o script, misturando as duas linguagens.

Detalhes sobre a linguagem PHP são que ela também toma por base a linguagem C, sendo visíveis algumas construções de comandos exatamente como em C, mas algumas regras foram modificadas em virtude das características de uso da linguagem como a inclusão do símbolo $ antes dos nomes de todas as variáveis, facilitando sua identificação, e agregação de *tags* HTML em meio ao código PHP como no comando *echo “</br>”;* que é responsável por exibir na tela o conteúdo entre aspas, assim como a função printf *()* em C, mas o conteúdo representa quebra de linha, tendo então a simples função de pular linha e não exibir texto.

Fonte: Freepik.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a05-img03.png)

Compreender o processo de elaboração de conteúdo web envolve o aprendizado de mais de uma linguagem e de como integrar os códigos e aplicações geradas por estas linguagens. É preciso estudar diferentes conceitos e ferramentas para que se possa ter sucesso no desenvolvimento de páginas, sites institucionais ou para comércio eletrônico, aplicativos para plataformas diversas e sistemas baseados na web.

Fonte:[Disponível aqui](https://www.w3schools.com/html/)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

Com isto, é possível observar que várias linguagens de programação compartilham aspectos semelhantes e facilitam seu aprendizado, mas todas elas necessitam de uma correta compreensão dos problemas a serem solucionados e uma precisa elaboração dos algoritmos capazes de proporcionar funcionalidades que atendam ao que se espera como solução.

## Linguagem GO

Mais recentemente, a Google, que pode ser considerada ainda uma empresa mais recente no mercado, desenvolveu a linguagem GO, de propósito geral e também baseada em C, para que pudesse servir como ferramenta de desenvolvimento de software e aplicativos otimizada para seu sistema operacional Android.

Essa linguagem rapidamente adquiriu vários adeptos em função de sua simplicidade e características próprias, fazendo com que tivesse uma participação relevante no mercado e tornando-se uma opção boa de aprendizado e busca de vagas de trabalho no mercado.

Possui como principal característica a possibilidade de desenvolvimento de software para a execução paralela de tarefas que podem ser definidas como outro paradigma chamado de programação concorrente.

Nessa forma de desenvolvimento de software, programas separados ou tarefas (*threads*) que sejam executadas paralelamente criadas por um programa, podendo ser executadas “ao mesmo tempo” pela divisão de tempo de processamento de um único processador ou pela execução das *threads* realmente em paralelo por vários processadores em um mesmo hardware, sendo que a pouco tempo foi criada a arquitetura de núcleos em um único processador que também podem ser programados para trabalharem paralelamente atendendo diferentes *threads* simultaneamente.

Mas esse recurso é opcional, e a linguagem pode agir tranquilamente como uma típica linguagem estruturada com sintaxe semelhante à linguagem C de uma forma otimizada e muito eficientes, tendo como uma importante característica, a possibilidade de uma função retornar mais de um valor ao final de sua execução, recurso não disponível normalmente nas demais linguagens populares do mercado. Veja:

package main

import "fmt"

func main() {

var lista = \[5\]int{10,20,30,40,50}

fmt.Println ("Lista inicial:", lista)

fmt.Scan (&lista \[2\])

fmt.Println ("Lista ajustada:", lista)

for i:= 0; i < 5; i++ {

lista \[i\] = lista \[i\] / 2

}

fmt.Println("Lista final: ", lista)

}

Fonte: autor.

Neste exemplo de código em linguagem GO, temos primeiramente a indicação de um pacote chamado **main**, conceito que permite o agrupamento de mais de um arquivo de código fonte em linguagem GO para compor um software mais complexo e modular.

É utilizada a palavra reservada **import** para incluir bibliotecas como a chamada **fmt** para funções de entrada e saída de dados como em C, onde funções como Println() e Scan() ou alternativas Print e Scanln() tendo como diferencial, que funções Println() e Scanln() mudam de linha na tela ao final de sua execução.

A declaração de um tipo de dado do tipo vetor para 5 números inteiros é declarada de uma forma diferente de C, e utilizando uma palavra reservada *var* antes da indicação do nome de uma variável para receber o vetor, seguindo da atribuição do vetor com valores de inicialização inseridos entre chaves.

Uma estrutura de repetição com base na palavra reservada **for** é gerada já com a declaração embutida de uma variável **i** de controle, inicializada com zero e sendo incrementada em uma unidade a cada iteração, podendo ser repetido enquanto o valor de **i** seja menor que 5, para ajustar uma a um, os elementos do vetor, dividindo os valores armazenados por 2.

A precedência de operadores é fundamental para que a lógica de algoritmos seja correta, mas para isso é importante conhecer a finalidade de cada tipo e operador específico e a partir da construção de expressões diversas mudando operadores e adicionando ou removendo parênteses, testar resultados a partir do ajuste da precedência.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Com a análise dos exemplos de diferentes linguagens de programação, temos diferentes ferramentas para codificação que podem ser utilizadas geralmente para o desenvolvimento de softwares para diferentes finalidades, mas que podem em alguns casos servirem de opções para o desenvolvimento de uma mesma solução, principalmente com linguagens de propósito geral.

Pode utilizar um software desenvolvido em Delphi para armazenar dados localmente para uma finalidade comercial, por exemplo, mas pode-se utilizar PHP com HTML para que essa mesma solução funcione como página web, e os dados podem ser armazenados na nuvem ou usar a linguagem GO para criar uma versão para dispositivos Android, todas utilizando como base os fundamentos da linguagem C.

 <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Linguagem Pascal
- Delphi
- Linguagem PHP
- Linguagem GO

Para complementar seus estudos, assista à videoaula a seguir: