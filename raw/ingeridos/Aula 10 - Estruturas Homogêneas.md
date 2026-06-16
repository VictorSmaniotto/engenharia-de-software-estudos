---
title: "Aula 10 - Estruturas Homogêneas"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-10.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 10 - Estruturas Homogêneas

Sumário[1\. Estruturas de Dados Homogêneas Unidimensionais](#topico-01)[

2\. Vetores

](#topico-02)

## Estruturas de Dados Homogêneas Unidimensionais

As estruturas de dados como vêm sendo estudadas ao longo deste material, representam um dos conceitos mais importantes no desenvolvimento de algoritmos, pois a ideia central dos algoritmos é o processamento de dados.

Até o momento foram utilizadas estruturas de dados simples para armazenamento de dados únicos em forma de variáveis que eram declaradas e tinham um tipo de dado atribuído para que estes tipos de dados declarados pudessem ser atribuídos a elas.

A partir desta aula, será ampliada a possibilidade de armazenamento temporário e manipulação de dados durante a execução de algoritmos por meio de um novo tipo de estrutura de dados.

Existe a possibilidade de se organizar uma maior quantidade de dados em forma de espécies de listas de dados de um mesmo tipo chamadas de estruturas de dados homogêneas.

Este tipo de estrutura pode ser declarado com um dos tipos de dados simples estudados, mas todos os elementos da estrutura deverão conter dados deste mesmo tipo a princípio.

Imagem ilustrativa.

[Disponível aqui](https://elements.envato.com/pt-br/codigo-de-programacao-Z9TC7DJ)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a10-img1.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/img-icon-quadrado-2.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/img-icon-bola-2.svg)

Existem linguagens de programação que não necessitam que um tipo de dado seja definido durante a declaração da variável e o tipo de dado acaba sendo dinamicamente definido ao longo da execução do *software* de acordo com o primeiro tipo de dado recebido, por exemplo.

Mas para os estudos neste material sempre será considerado o tipo definido logo na declaração de uma estrutura de dados para efeito em todo o algoritmo e entradas de dados de tipos incorretos ou atribuições de um tipo de dado para uma estrutura serão considerados erros em caso da execução de um algoritmo.

Quando forem realizados testes de mesa em algoritmos, é importante observar os tipos definidos e respeitá-los para melhor desenvolvimento dos testes, a menos que se queira buscar por erros em função da ausência de uma validação em entradas de dados.

Quando se imagina uma estrutura de dados homogêneas então, é preciso pensar numa sequência de variáveis todas de um mesmo tipo e nomeadas de forma única para efeitos de elaboração de algoritmos.

Este tipo de estrutura é interessante pela possibilidade de organizar listas de dados que podem ser adequadas para casos em que um mesmo tipo de dado ocorre diversas vezes em um algoritmo como no caso de listas de nomes de pessoas, números de senhas de espera, e qualquer tipo de lista de dados com um mesmo significado.

Este tipo de estrutura normalmente é nomeado como uma variável qualquer, mas seu identificador é acompanhado por um valor inteiro que define a quantidade máxima de dados suportados pela estrutura. Observe o exemplo a seguir.

| **1** | **2** | **3** | **4** | **5** | **6** | **7** | **8** | **9** | **10** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |  |  |

Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: O autor.

Pela representação gráfica trazida na imagem 30, percebe-se que cada elemento desse tipo de estrutura de dado homogênea reserva um espaço em memória para armazenamento de um único dado por vez, assim como ocorre com as variáveis.

Este tipo de estrutura possibilita várias funcionalidades adicionais ao que foi estudado até então, e simplifica a manipulação de uma maior quantidade de dados através de uma única estrutura de dados com um único nome.

Por meio de um índice associado a cada elemento da estrutura, esta pode ser facilmente manipulada pelas estruturas de controle para manipulação de seus dados, tornando este tipo de estrutura ideal para a organização de dados em forma de listas com quantidade limitada de elementos.

Laços de repetição podem ser utilizados para se mover pelos índices de uma estrutura de dados desse tipo, de forma sequencial para a realização de buscas, inserções de dados e edições, e estruturas condicionais podem permitir diferentes ações a serem realizadas com elementos da estrutura.

Este tipo de estrutura é chamada de vetor ou matriz unidimensional, mas para os estudos neste material, optou-se a utilização do termo vetor para diferenciação com matrizes que serão vistas em aula posterior.

## Vetores

Os vetores representam, então, estruturas de dados homogêneas que contêm uma quantidade pré-definida de dados de um mesmo tipo e que possuem índices para identificação de cada posição do vetor.

Para se trabalhar com vetores em algoritmos existe uma sintaxe que será adotada neste material para declarar e posteriormente para o uso destes em conjunto com os demais conteúdos estudados até o momento. Observe o exemplo da imagem 31 para conhecer a forma como será padronizada a declaração de vetores.

TIPO DADOS = VETOR \[1..100\] DE INTEIROS;

DADOS: LISTA;

Imagem 31: Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: O autor.

Neste exemplo de declaração de vetor contido na imagem 40, utiliza-se como base a sintaxe definida por Forbellone (2005), em que a palavra reservada “TIPO” para iniciar a declaração do tipo vetor, de forma que o mesmo possa ser utilizado como tipo para estruturas de dados desejadas num algoritmo.

O nome “DADO” é um identificador escolhido pelo desenvolvedor, e após o sinal de igualdade, é indicado que está sendo declarado um vetor com uma determinada quantidade de elementos em colchetes “\[1..100\]” do tipo inteiro indicado como “DE INTEIROS” para completar a instrução de definição do tipo vetor.

Na sequência, é declarada uma estrutura de dados “LISTA” com o uso do tipo definido “DADOS” da linha anterior para que seja então declarado um vetor com até 100 elementos.

O estudo de vetores é bastante interessante, pois permite que determinados tipos de aplicação possam ser implementados mais facilmente como listas de dados que permitam buscas e manipulações.

Acesse o link:[Disponível aqui](https://www.ime.usp.br/~pf/algoritmos/aulas/array.html)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

A manipulação de dados em vetores é bastante simples, mas é preciso que se tomem os devidos cuidados com a correta utilização da estrutura, pois erros na elaboração de algoritmos que manipulem estas estruturas podem acarretar perdas de maiores volumes de dados.

INÍCIO

DECLARE

TIPO DADOS = VETOR \[1..10\] DE INTEIROS;

DADOS: LISTA;

INTEIRO: I, BUSCA;

PARA I DE 1 ATÉ 10 PASSO 1 FAÇA

LEIA (LISTA \[ I \]);

FIMPARA;

ESCREVA (“DIGITE UM VALOR PARA BUSCA NO VETOR: “);

LEIA (BUSCA);

PARA I DE 1 ATÉ 10 PASSO 1 FAÇA

SE (LISTA \[I\] = BUSCA) ENTÃO

ESCREVA (“VALOR ENCONTRADO NA POSIÇÃO “, I);

FIMSE;

FIMPARA;

FIM.

Imagem 32: Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: O autor.

No algoritmo exemplo da imagem 32, é declarado um tipo vetor de inteiros chamado “DADOS” com até 10 números para exemplificar a criação e uso de uma lista de números inteiros. Em seguida, uma variável “LISTA” é declarada a partir do tipo “DADOS” definido. Na sequência, um laço de repetição é utilizado para que dados sejam inseridos com o comando “LEIA” em todas as dez posições possíveis do vetor.

Depois, numa próxima etapa, é solicitado ao usuário que digite um número a ser pesquisado no vetor que será armazenado na variável “BUSCA” para dentro de outro laço de repetição que passará por todo o vetor, ter seu valor comparado com o valor armazenado em cada posição do vetor. Caso seja encontrado um valor do vetor igual ao da variável que armazena o número indicado pelo usuário, uma mensagem informando a posição onde estava o valor igual é exibida.

Os vetores são estruturas muito úteis em situações em que seja necessário o armazenamento de listas de dados, mas sua manipulação necessita de treino para que seja possível a inserção de estruturas deste tipo em algoritmos sem que a complexidade de uso destas estruturas se torne um problema.

A ideia é criar estruturas homogêneas com tamanhos diversos e tipos variados para se conhecer os meios de manipulação para cada tipo de dado e saber trabalhar com os índices que identificam os elementos em vetores.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

Uma variação para o algoritmo trazido na imagem 33 é mostrada na imagem 41 que altera uma das estruturas de controle para que o algoritmo se torne mais eficiente em sua execução.

INÍCIO

DECLARE

TIPO DADOS = VETOR \[1..10\] DE INTEIROS;

DADOS: LISTA;

INTEIRO: I, BUSCA;

PARA I DE 1 ATÉ 10 PASSO 1 FAÇA

LEIA (LISTA \[ I \]);

FIMPARA;

ESCREVA (“DIGITE UM VALOR PARA BUSCA NO VETOR: “);

LEIA (BUSCA);

I <- 1;

ENQUANTO (LISTA \[I\] <> BUSCA OU I <= 10) FAÇA

SE (LISTA \[I\] = BUSCA) ENTÃO

ESCREVA (“VALOR ENCONTRADO NA POSIÇÃO “, I);

FIMSE;

I <- I + 1;

FIMENQUANTO;

FIMPARA;

FIM.

Imagem 33: Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: O autor.

Nesta variação de algoritmo da imagem 33, após a mesma definição de tipo vetor, declaração de variável vetor, e preenchimento dos dados no mesmo, como uma primeira etapa do algoritmo, a segunda parte sofreu alterações.

Após a solicitação do número a ser pesquisado, a variável “I” é reinicializada com valor 1 e um laço de repetição condicional substitui o contado, e com a possibilidade indicada de interrupção das iterações baseadas ou na ausência de número igual no vetor ao solicitado, ou não término do vetor, a estrutura segue por cada posição do vetor comparando os valores e controlando a quantidade de iterações realizadas com o incremento manual em uma unidade da variável contadora a cada iteração.

  <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Estruturas de Dados Homogêneas Unidimensionais
- Vetores

Para complementar seus estudos, assista à videoaula a seguir: