---
title: "Aula 13 - Programação Lógica - Conceitos"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-13.html"
author:
published:
created: 2026-06-18
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 13 - Programação Lógica - Conceitos

Baseada na lógica formal, ramo da matemática, utilizam-se diversos conceitos dessa área para a definição do paradigma lógico, e consequentemente, as linguagens baseadas neste paradigma também possuem conceitos adaptados da lógica formal.

## Lógica Formal

Segundo Sebesta (2011), um dos conceitos fundamentais deste paradigma são as proposições que são compostas por sentenças lógicas que podem resultar verdadeiras ou falsas, sendo que a base para estas sentenças é a construção de relacionamentos entre elementos.

Existe também um forte uso de símbolos para a construção de proposições de forma que neste paradigma, muitos dos símbolos matemáticos utilizados na programação mudam seu grau de relevância em relação a outros paradigmas.

Os elementos (objetos) utilizados na composição de proposições podem ser representados por termos simples, variáveis ou até constantes como nos demais paradigmas de uma forma similar, mas com características um pouco distintas.

Uma constante é um símbolo que representa um objeto. Uma variável é um símbolo capaz de representar objetos diferentes em momentos diferentes, apesar de, em certo sentido, essas variáveis serem muito mais próximas da matemática do que as variáveis em uma linguagem de programação imperativa. (Sebesta, 2011).

As proposições podem ser simples ou compostas, e uma proposição simples é mais fácil de ser construída e avaliada, pois existe apenas uma avaliação a ser feita como verdadeira ou falsa apenas, ao passo que numa proposição composta, mais de uma proposição simples precisa ser avaliada e se torna necessário um elemento adicional para que os resultados das proposições simples possam ser avaliados em conjunto.

Para realizar a avaliação das proposições simples em uma proposição composta, é preciso que sejam utilizados operadores lógicos representados por símbolos para que os resultados das proposições simples sejam avaliados como verdadeiras ou falsas e representam o resultado da proposição composta.

Na lógica os operadores podem representar negação, conjunção, disjunção, equivalência ou implicação, mas na programação, nem todos os mesmos conceitos são utilizados e alguns símbolos podem ser diferentes. Observe os principais símbolos matemáticos e seus significados na imagem a seguir:

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a13-fig01.jpg)

Fonte: Sebesta (2011).

Expressões como “a ⊃ b ou “a ∩ b” são muito comuns na matemática como relações entre elementos de conjuntos, mas também podem representar as operações lógicas E e OU que são operações lógicas muito comuns na programação.

Observe a tabela verdade na imagem a seguir para compreender como são avaliados os operadores quanto aos resultados que podem ser obtidos com proposições verdadeiras ou falsas.

| **P** | **q** | **p ^ q** |
| --- | --- | --- |
| **V** | **V** | **V** |
| **V** | **F** | **F** |
| **F** | **V** | **F** |
| **F** | **F** | **F** |

Fonte: O autor.

Na imagem acima, pode ser observado que somente quando ambas as proposições simples resultam verdadeiro, a aplicação da conjunção entre estes valores resulta também verdadeiro.

O mesmo vale para disjunções que representam o operador OU e somente resultam em falso no caso de todos os resultados de proposições simples são falsas como é mostrado na imagem a seguir.

| **P** | **q** | **p v q** |
| --- | --- | --- |
| **V** | **V** | **V** |
| **V** | **F** | **V** |
| **F** | **V** | **V** |
| **F** | **F** | **F** |

Fonte: O autor.

Para melhor compreender os fundamentos do uso de operadores para a construção de proposições, é importante consultar materiais de aplicação de operadores lógicos. Geralmente associam-se tabelas verdade aos operadores lógicos para mostrar como um operador E resulta verdadeiro apenas se todos os valores avaliados pelo operador sejam verdadeiros, ou no caso do operador OU, pelo menos um valor precisa ser verdadeiro para que toda a proposição seja verdadeira.

Fonte:[Disponível aqui](https://educacao.uol.com.br/disciplinas/portugues/giria-e-jargao-a-lingua-mudaconforme-situacao.htm)

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Termos compostos são representações de funções com sintaxe similar à utilizada em outros paradigmas e suas linguagens e representam as principais estruturas em linguagens de programação baseadas no paradigma lógico.

## Paradigma Lógico

Este paradigma trabalha com proposições atômicas compostas por relações semelhantes à da sintaxe de programação funcional onde duas partes compõe a sintaxe, e é a relação e uma lista de elementos entre parênteses que componham esta relação.

homem (joao).

mulher (maria).

casados (joao,maria).

Fonte: autor.

Pelo exemplo de termos compostos contidos nos exemplos da imagem, temos diferentes situações, em que os dois primeiros exemplos apresentam fatos, pois indicam que determinada relação se aplica a determinado elemento indicado dentro dos parênteses.

As proposições atômicas são uma nomenclatura que pode ser utilizada nestes casos onde a combinação de símbolos de predicados com termos simples ou compostos indicados entre parênteses como mostrado na última imagem.

No terceiro exemplo, existe um tipo diferente de relação onde dois elementos são relacionados entre si a partir da função indicada, e da mesma forma que num termo com apenas um parâmetro, pode ser verdadeiro ou falso.

Linguagens que se baseiam no paradigma lógico são ditas declarativas e são de certa forma mais simples que linguagens imperativas em termos de semântica, mas com menor variedade de soluções computacionais possíveis, sendo por isto mais limitada no mercado.

Por ser um paradigma não procedural, o paradigma foca na forma dos resultados de processamentos realizados e não tanto no processamento em si, fazendo com que o programador não tenha tanto controle sobre o processo em si como no paradigma imperativo onde toda a sequência de ações é determinada sequencialmente.

Em linguagens procedurais, um algoritmo deve ser aplicado sobre dados que contém uma sequência de ações a serem realizadas até que todo o processo esteja concluído e algum resultado desejado seja obtido, ou não seja possível a obtenção de resultados desejáveis por quaisquer problemas.

Em linguagens não procedurais, apenas as características dos elementos que contêm dados devem ser descritos e as relações entre eles, de forma que se possa trabalhar estes dados e obter ou não os resultados esperados, como na ordenação de elementos de uma lista que necessitam apenas que os adjacentes sejam comparados com base em uma relação que trabalhe estes dados.

Áreas como a de banco de dados podem utilizar em suas buscas determinadas estruturas de dados que servem de índices e podem ser utilizadas em conceitos de lógica e mecanismos presentes no paradigma lógico para obter melhor desempenho. Para grandes volumes de dados, o uso de relações algébricas pode ser muito vantajoso dependendo de como for implementado o mecanismo para uso adequado dos recursos de hardware também. Também pode ser utilizado em aplicações voltadas à área de inteligência artificial e aprendizado de máquina devido à possibilidade de se obter novos conhecimentos a partir da construção de novas relações a partir das proposições já existentes.

![início da abordagem prática](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-abordagem-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Lógica Formal
- Paradigma Lógico

Para complementar seus estudos, assista à videoaula a seguir: