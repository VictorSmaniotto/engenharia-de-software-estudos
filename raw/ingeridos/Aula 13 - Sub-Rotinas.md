---
title: "Aula 13 - Sub-Rotinas"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-13.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 13 - Sub-Rotinas

Sumário[1\. Sub-Rotinas](#topico-01)[

2\. Escopo de Estruturas de Dados

](#topico-02)[

3\. Procedimentos

](#topico-03)[

4\. Funções

](#topico-04)

## Sub-Rotinas

Existem os chamados paradigmas de programação que definem diferentes formas de se programar, e até este momento nos estudos foi utilizado um paradigma chamado imperativo em que o algoritmo inicia em um bloco de instruções que se seguem até o final contendo todas as funcionalidades do mesmo.

Nesta aula será trabalhada uma nova forma de se construir algoritmos com base em outro paradigma. O paradigma estruturado permite que partes de um algoritmo sejam inseridos em sub-rotinas que possam ser acessadas pela parte principal deste algoritmo a qualquer momento, reduzindo a quantidade de linhas necessárias em algoritmos mais complexos e oferecendo uma maior possibilidade de reuso de código no desenvolvimento de outros algoritmos, posteriormente.

Uma sub-rotina representa um nome que se refere a todo um trecho de código com certa independência de funcionalidades em relação ao restante de um algoritmo e se torna algo como se um algoritmo fosse aninhado dentro de outro, como foi estudado com estruturas de controle em aulas anteriores.

Dentro de uma sub-rotina é possível utilizar praticamente todos os conceitos estudados até este ponto e criar algoritmos cada vez mais eficientes e mais bem organizados e fáceis de interpretar e modificar quando necessário.

Forbellone (2005) utiliza o termo módulo para todo tipo de sub-rotina, mas existem dois tipos de sub-rotinas para diversos autores e linguagens de programação, e em função desta possibilidade de separação entre tipos de sub-rotinas, será usada a definição citada por Manzano (1997) que organiza as sub-rotinas em procedimentos e funções.

Imagem ilustrativa | Fonte: seventyfourimages

[Disponível aqui](https://elements.envato.com/pt-br/codificador-talentoso-trabalhando-com-linguagem-3G9XC76)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a13-img1.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/img-icon-quadrado-2.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/img-icon-bola-2.svg)

## Escopo de Estruturas de Dados

O chamado escopo de estruturas de dados é um importante conceito a ser trabalhado neste ponto dos estudos, pois afeta diretamente o uso e funcionalidades de sub-rotinas, podendo tornar um pouco mais complexa a compreensão das sub-rotinas e como utilizá-las corretamente.

Escopo se refere a qual ponto em um algoritmo uma estrutura de dados pode ser utilizada diretamente, e quando é necessário que referências a estruturas de dados sejam feitas para que se possa acessar seus dados e manipulá-los.

Para esta aula serão desconsiderados os meios para se transmitir dados entre sub-rotinas, pois é conteúdo para a aula seguinte, mas é importante saber que para se utilizar sub-rotinas quaisquer, não é obrigatória a declaração de estruturas de dados todas globais que possam ser acessadas de quaisquer pontos de um algoritmo para solucionar todos os problemas.

O ideal é que se complemente os conteúdos trabalhados nesta aula com os da aula seguinte para que o conjunto desses conceitos se torne uma ferramenta muito eficiente de desenvolvimento de algoritmos e software em diversas linguagens de programação.

Atuando apenas com as estruturas de dados declaradas de acordo com seus respectivos escopos apenas, é preciso um planejamento para a construção de algoritmos de forma que os dados possam ser utilizados de maneira adequada pelo algoritmo, o uso de estruturas de dados em algoritmos serão tratados agora da seguinte maneira:

- Estruturas de dados declaradas na parte principal do algoritmo são tratadas como globais, ou seja, acessíveis de qualquer ponto do algoritmo.
- Estruturas de dados locais declaradas dentro de sub-rotinas podem apenas ser acessadas por instruções contidas na sub-rotina onde foi declarada, ficando assim, inacessível em outros pontos do algoritmo.

O uso de variáveis e outras estruturas internamente a sub-rotinas é bastante comum, mas é preciso lembrar que qualquer estrutura de dados declarada dentro de uma sub-rotina se torna local a ela.

Assim, é preciso estar ciente de que dados gerados em sub-rotinas e armazenados em estruturas locais são todos perdidos quando se sai de uma sub-rotina e retorna-se ao trecho do algoritmo que chamou a sub-rotina.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

## Procedimentos

O princípio dos dois tipos de sub-rotina é o mesmo, mas os procedimentos em si são mais simples de se compreender e de utilizar, pois possuem menos detalhes a serem implementados.

Os procedimentos são sub-rotinas que executam processamento de dados com base em dados obtidos de estruturas de dados que sejam de escopo global, pois estruturas de dados que sejam de fora do procedimento e sejam considerados de escopo local não podem ser acessados pelo procedimento, a menos que sejam passados para o procedimento como será visto na aula seguinte.

Os procedimentos são sub-rotinas que executam processamento de dados de forma interna e podem atuar no restante do algoritmo fora da sub-rotina apenas se estruturas de dados globais forem manipuladas, e estruturas de dados contidas em outros procedimentos não podem ser acessados por terem escopo local.

Observe na imagem 40 um exemplo de procedimento que pode ser inserido em qualquer algoritmo, desde que suas funcionalidades e estruturas de dados necessárias para que possa ser executado sejam respeitadas.

PROCEDIMENTO CALCULA ()

DECLARE

INTEIRO: SOMA;

SOMA <- V1 + V2 + V3;

ESCREVA (“RESULTADO = “, SOMA);

FIM;

Imagem 40: Exemplo de procedimento. | Fonte: O autor.

Neste exemplo da imagem 40, é declarado um procedimento por meio da palavra reservada “PROCEDIMENTO” seguido de um nome e parênteses. Esta sintaxe para procedimentos foi padronizada com base na sintaxe de Manzano (1997), mas ajustada para se aproximar também da sintaxe trazida por Ascencio (2011).

Com esses ajustes nas sintaxes trazidas por diferentes autores, obteve-se esta sintaxe que se assemelha a do desenvolvimento para o algoritmo padrão estudado nas aulas anteriores, e assim, é mais fácil compreender a ideia de que uma sub-rotina pode ser vista como se fosse um pequeno algoritmo que pode ser chamado por outro algoritmo num mesmo arquivo.

Neste exemplo trazido na imagem 40, é declarado um procedimento chamado “CALCULA” que possui declarada, logo em seguida, uma variável “SOMA” definida como número inteiro. Depois, esta variável “SOMA” recebe os valores contidos nas variáveis “V1”, “V2”, e “V3” para obter um resultado atribuído à variável “SOMA”.

As três variáveis utilizadas no cálculo não foram declaradas no procedimento “CALCULA” como a variável para o resultado, e assim, supõe-se que, ou as variáveis foram declaradas no algoritmo principal e são de escopo global, ou foram esquecidas as declarações destas três variáveis. Em seguida, após a obtenção do resultado para o cálculo, é exibido ao usuário o valor obtido em uma mensagem, para depois, o procedimento ser encerrado, e o controle do fluxo de execução do algoritmo ser retomado pelo algoritmo principal.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg)

## Funções

As funções possuem uma característica importante que as diferem dos procedimentos, pois possuem um tipo de dado associado à própria função e que ao final da execução da mesma, deve então retornar um valor para o trecho do algoritmo que chamou a função.

Em razão desta diferença, a forma como se deve chamar uma função também ocorre de forma diferente, pois os procedimentos, por não retornarem valor nenhum, é chamado simplesmente pelo seu nome no algoritmo, ao passo que uma função, pelo retorno que deve efetuar, deve estar associada a uma atribuição de valor, a uma estrutura de dados ou como parte de uma instrução de saída de dados.

Assim, a partir de uma adaptação da sintaxe trazida por Ascencio (2011), a sintaxe para uso neste material se assemelhará ao da sintaxe dos procedimentos, tendo como diferencial, a definição do tipo e retorno de valor ao final da função. Observe o exemplo da imagem 41.

FUNÇÃO CALCULA () DE INTEIRO

DECLARE

INTEIRO: SOMA;

SOMA <- V1 + V2 + V3;

ESCREVA (“RESULTADO = “, SOMA);

RETORNE SOMA;

FIM;

Imagem 41: Exemplo de função. | Fonte: O autor.

Por este exemplo da imagem 41, percebe-se que é uma adaptação do procedimento da imagem 40, de forma a torná-lo uma função, e para isto, a modificação ocorre na palavra reservada “FUNÇÃO” inserida antes do nome da sub-rotina, e do acréscimo da palavra reservada “DE” seguido de um tipo válido de dados para definir o retorno na função.

O processamento interno da função se mantém igual, e ao final, antes do “FIM” da função, utiliza-se a palavra reservada “RETORNE”, seguida do valor a ser retornado ao trecho do algoritmo que chamou a função. Detalhe que o valor a ser retornado pode ser um dado em si, ou uma estrutura de dados para que o valor contido na mesma seja retornado.

Como estamos lidando com algoritmos, e não uma linguagem em si, não há muitas limitações na elaboração de algoritmos na verdade, mas para efeito de estudos, padrões são definidos para simplificar os estudos, mas é possível ampliar os conceitos para que sejam mais abrangentes, e assim, pode-se, por exemplo, utilizar vetores, matrizes ou registros como tipos válidos para funções e seus retornos, tornando a elaboração de algoritmos mais complexa e completa, mesmo que muitas linguagens não possuam essa capacidade de lidar com funções assim.

O uso de funções em programação é muito comum, e a estruturação de código em funções é inclusive foco de uma forma de programação que se baseia na implementação de funções para todas as funcionalidades. O chamado paradigma de programação funcional trabalha com funções como base de toda a programação, assim como nos cálculos matemáticos.

Acesse o link:[Disponível aqui](https://www.infoq.com/br/fp/)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Sub-Rotinas
- Escopo de Estruturas de Dados
- Procedimentos
- Funções

Para complementar seus estudos, assista à videoaula a seguir: