---
title: "Aula 11 - Estruturas Homogêneas Multidimensionais"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-11.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 11 - Estruturas Homogêneas Multidimensionais

Sumário[1\. Matrizes](#topico-01)[

2\. Aplicação Prática de Matrizes

](#topico-02)

## Matrizes

Uma estrutura multidimensional homogênea possui diversas finalidades práticas como armazenamento temporário, e em certos casos é até difícil imaginar seu uso, mas a base para muitos softwares são matrizes.

Um exemplo importante é a própria formação da uma imagem na tela de um computador. As imagens são formadas por pixels que podem ser representados por matrizes.

Assim, em uma tela com resolução 1024x768 pixels, por exemplo, é possível representar cores que poderiam ser inseridas em cada ponto da tela com um valor que pode representar a cor relativa a cada pixel responsável por compor uma imagem.

Mesmo na exibição de vídeos, a ideia da matriz se mantém, pois uma imagem estática é facilmente interpretada como uma matriz de valores, mas é preciso compreender que um vídeo também é composto por imagens estáticas que são trocadas a determinada velocidade medida em quadros (imagens) por segundo. Observe a imagem 34 para um exemplo de imagem.

| **XY** | **1** | **2** | **3** | **4** | **5** | **6** | **7** | **8** | **9** | **10** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **1** | 0 | 0 | 0 | 50 | 50 | 50 | 50 | 0 | 0 | 0 |
| **2** | 0 | 0 | 50 | 50 | 50 | 50 | 50 | 50 | 0 | 0 |
| **3** | 0 | 0 | 50 | 50 | 50 | 50 | 50 | 50 | 0 | 0 |
| **4** | 0 | 0 | 50 | 50 | 20 | 50 | 20 | 50 | 0 | 0 |
| **5** | 0 | 0 | 50 | 50 | 50 | 35 | 50 | 50 | 0 | 0 |
| **6** | 0 | 0 | 50 | 50 | 50 | 50 | 50 | 50 | 0 | 0 |
| **7** | 0 | 0 | 50 | 50 | 20 | 20 | 20 | 50 | 0 | 0 |
| **8** | 0 | 0 | 50 | 50 | 50 | 50 | 50 | 50 | 0 | 0 |
| **9** | 0 | 0 | 0 | 50 | 50 | 50 | 50 | 0 | 0 | 0 |
| **10** | 0 | 0 | 0 | 50 | 50 | 50 | 50 | 0 | 0 | 0 |

Imagem 34: Matriz representativa de uma imagem com 10x10 pixels. | Fonte: O autor.

Na representação da matriz na imagem 34, observa-se que temos 10 linhas e 10 colunas representando uma estrutura de dados para números com a possibilidade de armazenamento temporário de até 100 valores pela multiplicação simples entre a quantidade de linhas e colunas.

Pela disposição dos valores na matriz, é possível perceber que apenas na posição indicada pela linha 5 e coluna 6, temos o único valor 35 na matriz, servindo de exemplo para a compreensão do uso de índices de linha e coluna para indicação de dados em uma matriz. Neste caso, 5x6.

Outra aplicação comum é para a elaboração de jogos de tabuleiro em que matrizes podem conter peças indicadas por números representativos de peças a serem movimentadas. Xadrez, damas, e outros tipos como palavras cruzadas, por exemplo.

Jogos mais complexos também podem ser elaborados com base em matrizes cuja ideia de posicionar elementos pela tela se mantém e diversos tipos de informações podem ser inseridos neste tipo de estrutura como a posição de elementos espalhados pela matriz, ou seja, pela tela de jogo. Observe a imagem 35 para um exemplo de jogo que pode ter seus elementos dispostos em uma matriz de duas dimensões.

![ a imagem mostra a tela de um jogo clássico, o Space Invaders, com suas naves coloridas no fundo preto. ](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a11-img1.jpg)

Imagem 35: Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: [Disponível aqui](https://pixabay.com/pt/illustrations/plano-de-fundo-v%C3%ADdeo-game-3311042/)

Na imagem 35, é possível imaginar os elementos que se movem pela tela sendo controlados a partir de referências indicadas numa matriz que serve de base para que todas as posições dos elementos sejam conhecidas e possam ser modificadas durante o jogo.

Para se declarar uma estrutura que possa ser utilizada para matrizes, a sintaxe básica inicia pela palavra reservada “TIPO”, seguida pelo nome escolhido para a matriz. Em seguida utiliza-se sempre a sequência “= MATRIZ” e as dimensões e intervalo de valores aceitos na forma “\[1..N\]\[1..M\]...\[1..Z\]”, em que cada par de colchetes indicam uma dimensão. Por fim, inclui-se depois a palavra reservada “de” e finalmente um tipo de dado para declarar a estrutura e o ponto e vírgula padrão da sintaxe. Observe os exemplos da imagem 36.

TIPO TABULEIRO = MATRIZ \[1..8\]\[1..8\] DE CARACTERES;

TIPO VELHA = MATRIZ \[1..3\]\[1..3\] DE CARACTERES;

TIPO CUBOMAGICO = MATRIZ \[1..3\]\[1..3\]\[1..3\] DE INTEIRO;

Imagem 36: Exemplos de declaração de matrizes. | Fonte: O autor.

Nos exemplos trazidos na imagem 36 temos as declarações de matrizes para situações bastante comuns como para um tabuleiro de damas ou xadrez no primeiro caso com 8 linhas e 8 colunas. No segundo exemplo, é declarada uma matriz chamada “VELHA” que pode ser usada como base para um jogo da velha, e por fim, no terceiro exemplo, uma matriz de três dimensões que pode ser base para a implementação de um cubo mágico.

Estruturas de dados homogêneas são importantes para o desenvolvimento de algoritmos e permitem que em uma ou mais dimensões, dados sejam armazenados e manipulados de forma organizada. Procurem sempre aprofundamentos no uso deste tipo de estrutura de dados.

Acesse o link:[Disponível aqui](http://fabrica.ms.senac.br/2013/06/algoritmo-estrutura-de-vetores-e-matrizes/)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Aplicação Prática de Matrizes

Para um exemplo completo de uso de matriz, foi escolhido como tema o jogo da velha que é bastante simples em suas regras, compreensão e adaptação para algoritmo, sendo então um bom exemplo a ser desenvolvido e compreendido.

Foi escolhida uma sintaxe alternativa que pode ser utilizada no *software* VisualG 3.0 disponível em https://sourceforge.net/projects/visualg30/. Esta ferramenta permite a execução de algoritmos em português e foi desenvolvida pelo professor Antonio Carlos Nicolodi. Observe a imagem 45 para conhecer a interface da ferramenta de interpretação de algoritmos.

![a imagem mostra a tela do software VisualG.](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a11-img2.jpg)

Imagem 45: Exemplo de estrutura de decisão em estrutura de repetição. | Fonte: O autor.

A sintaxe para a ferramenta é um tanto distinta em relação ao que está sendo estudado, mas a lógica em si se mantém a mesma, servindo perfeitamente como exemplo para interpretação e teste de um algoritmo completo e funcional que pode ser jogado. A seguir, na imagem 37, temos o algoritmo completo para estudos e teste na ferramenta, se desejado.

ALGORITMO "JOGO DA VELHA"

VAR

MATRIZ: VETOR \[1..3,1..3\] DE CARACTERE

I, J, JOGADOR, RODADAS: INTEIRO

INÍCIO

JOGADOR <- 1

RODADAS <- 0

// Inicialização da matriz para que todas as posições estejam em branco.

PARA I DE 1 ATE 3 PASSO 1 FACA

PARA J DE 1 ATE 3 PASSO 1 FACA

MATRIZ \[I,J\] <- " "

FIMPARA

FIMPARA

// Laço de repetição que para só se alguém ganha ou acabam os espaços.

ENQUANTO (RODADAS <= 9) FACA

// Desenha o jogo da velha atualizado.

ESCREVAL (" \*\*\* JOGO DA VELHA \*\*\*")

PARA I DE 1 ATE 3 PASSO 1 FACA

ESCREVAL (MATRIZ\[I,1\], " | ", MATRIZ\[I,2\], " | ", MATRIZ\[I,3\])

SE (I < 3) ENTAO

ESCREVAL ("--+---+--")

FIMSE

FIMPARA

// Solicita as coordenadas dos jogador a cada rodada.

ESCREVA ("DIGITE A LINHA DESEJADA: ")

LEIA (I)

ESCREVA ("DIGITE A COLUNA DESEJADA: ")

LEIA (J)

SE (JOGADOR = 1) ENTAO

MATRIZ \[I,J\] <- "X"

JOGADOR <- 2

SENAO

MATRIZ \[I,J\] <- "O"

JOGADOR <- 1

FIMSE

RODADAS <- RODADAS + 1

// Inicia a avaliação de vitória de cada jogador a cada rodada.

SE ((MATRIZ\[1,1\] = "O") E (MATRIZ\[1,2\] = "O") E (MATRIZ\[1,3\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[2,1\] = "O") E (MATRIZ\[2,2\] = "O") E (MATRIZ\[2,3\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[3,1\] = "O") E (MATRIZ\[3,2\] = "O") E (MATRIZ\[3,3\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,1\] = "O") E (MATRIZ\[2,1\] = "O") E (MATRIZ\[3,1\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,2\] = "O") E (MATRIZ\[2,2\] = "O") E (MATRIZ\[3,2\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,3\] = "O") E (MATRIZ\[2,3\] = "O") E (MATRIZ\[3,3\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,1\] = "O") E (MATRIZ\[2,2\] = "O") E (MATRIZ\[3,3\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,3\]= "O") E (MATRIZ\[2,2\] = "O") E (MATRIZ\[3,1\] = "O")) ENTAO

ESCREVAL ("JOGADOR 2, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,1\] = "X") E (MATRIZ\[1,2\] = "X") E (MATRIZ\[1,3\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[2,1\] = "X") E (MATRIZ\[2,2\] = "X") E (MATRIZ\[2,3\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[3,1\] = "X") E (MATRIZ\[3,2\] = "X") E (MATRIZ\[3,3\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,1\] = "X") E (MATRIZ\[2,1\] = "X") E (MATRIZ\[3,1\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,2\] = "X") E (MATRIZ\[2,2\] = "X") E (MATRIZ\[3,2\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,3\] = "X") E (MATRIZ\[2,3\] = "X") E (MATRIZ\[3,3\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,1\] = "X") E (MATRIZ\[2,2\] = "X") E (MATRIZ\[3,3\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

SE ((MATRIZ\[1,3\] = "X") E (MATRIZ\[2,2\] = "X") E (MATRIZ\[3,1\] = "X")) ENTAO

ESCREVAL ("JOGADOR 1, VOCÊ VENCEU!!!")

RODADAS <- 10

FIMSE

// Esta opção é para o caso de ser preenchida a matriz sem vitorioso.

SE (RODADAS = 9) ENTAO

ESCREVAL ("PARTIDA EMPATADA!!!")

FIMSE

FIMENQUANTO

FIMALGORITMO

Imagem 37: Exemplo jogo da velha para aplicação na ferramenta VisualG. | Fonte: O autor.

Neste exemplo da imagem 37, temos um algoritmo implementado para simular uma versão simples do jogo da velha no qual primeiramente é declarada uma matriz de caracteres com 3 linhas e 3 colunas chamada “MATRIZ” para conter os caracteres “X” e “O” utilizados a cada rodada no jogo.

Depois são declaradas as variáveis “I” e ”J” do tipo inteiro para serem utilizadas como índices para posicionamento na matriz que representa o jogo em si para armazenamento dos símbolos que representam as coordenadas escolhidas por cada jogador a cada rodada.

Outra variável chamada “JOGADOR” é declarada para indicar a vez de quem está jogando poder informar as coordenadas de seu palpite a cada rodada. Na sequência do algoritmo, é utilizada uma instrução de atribuição para a variável “JOGADOR” para indicar quem iniciará a partida.

Por fim, a variável “RODADAS” é declarada para conter a quantidade de rodadas já jogadas e também para ser utilizada e saber se o jogo chegou ao fim sem vencedor, fato que encerra a estrutura de repetição condicional e também se chega ao final da execução do algoritmo.

Outra inicialização é feita por segurança utilizando um laço de repetição aninhado dentro de outro para percorrer toda a matriz, atribuindo um espaço em branco como dado para que não haja risco de a estrutura conter dados indevidos ou até “X” ou “O” por coincidência. Em um algoritmo não é algo essencial, mas em muitas linguagens de programação é uma prática que melhora a funcionalidade adequada de um *software*.

Na sequência, inicia-se um laço de repetição controlado pela variável “RODADAS” em que é verificado se o valor da variável “RODADAS” já atingiu o valor limite 9 que representa a matriz cheia de “X” ou “O”. Este laço de repetição é fundamental, pois ele controla o jogo em si a cada rodada até que haja um vencedor ou a matriz seja toda preenchida sem um vencedor.

Dentro do laço, inicialmente é utilizado um pequeno laço para desenhar o jogo da velha para que o usuário possa acompanhar o andamento do jogo e para melhorar a interface, mesmo que de forma simples e textual.

Depois, são pedidas as coordenadas (linha e coluna) a serem preenchidas com “X” ou “O” de acordo com a vez de cada participante, controladas pela variável “JOGADOR” que alterna de valor a cada rodada, ao mesmo tempo em que as coordenadas informadas são utilizadas para o preenchimento da posição da matriz correspondente com o símbolo correspondente de cada jogador.

Em seguida, entra uma parte grande do código onde cada possibilidade de vitória do jogador representado pelo símbolo “O” é verificada (linhas, colunas ou diagonais com o mesmo símbolo), e caso ocorra, o valor da variável “RODADAS” é atualizado para 10 para que seja encerrado o laço de repetição, ao mesmo tempo em que é exibida uma mensagem de vitória ao jogador.

O mesmo é feito para o outro jogador, com base nas mesmas regras, mudando apenas o símbolo para “X” e a mensagem sendo adequada ao outro jogador vitorioso, caso ocorra uma das possibilidades.

Por fim, é feita uma verificação se a matriz não foi preenchida sem vitorioso com a quantidade de rodadas chegando a 9 e sem nenhuma das condições de vitória tendo sido atendida, informando aos usuários que não houve vencedor.

Com esse exemplo da imagem 46, é possível perceber que os algoritmos representam importante ferramenta de aprendizado da programação e podem auxiliar em posterior estudo de qualquer linguagem de programação, pois a lógica em si se mantém, bastando adaptações de sintaxe para adequação aos padrões de cada diferente linguagem.

Uma boa prática para melhor aprendizado deste tipo de estrutura de dados é a implementação de mudanças em códigos testados para mudar funcionalidades, acrescentar validações de dados, alterar dimensões e limites na quantidade de dados por dimensão, etc.

Da mesma forma que foi trazido um exemplo de algoritmo para o jogo da velha utilizando matriz, pode-se, além de alterar seu algoritmo para acréscimo de melhorias e validações para o preenchimento da matriz, assim como tentar novos algoritmos usando matrizes como caça-palavras, batalha naval, etc.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Matrizes
- Aplicação Prática de Matrizes

Para complementar seus estudos, assista à videoaula a seguir: