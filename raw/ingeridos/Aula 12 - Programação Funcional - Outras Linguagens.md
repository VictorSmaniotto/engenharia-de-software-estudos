---
title: "Aula 12 - Programação Funcional - Outras Linguagens"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-12.html"
author:
published:
created: 2026-06-18
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 12 - Programação Funcional - Outras Linguagens

A linguagem Lisp é a linguagem mais antiga que utiliza o paradigma funcional e evoluiu com o tempo, mas mesmo assim não representa a linguagem mais popular e também mais completa.

## Linguagem Lisp

Como citado anteriormente, esta linguagem utiliza dois tipos de estruturas para dados em sua versão original, sendo elas átomos que representam elementos puros como letras ou números, por exemplo, e listas que representam conjuntos formados por átomos e listas que também podem ser utilizadas como elementos de outra lista.

As funções são escritas de forma simples, com uma sintaxe básica onde é indicada uma função matemática como primeiro átomo dentro dos parênteses e depois, os demais átomos a serem utilizados na função. A função (+ 5 5) é um exemplo que retornaria o valor 10 como resultado da soma dos átomos 5 e 5.

Com o tempo, novas formas de construção de código em Lisp foram implementadas para que funções pudessem ser vinculadas a outras funções como no exemplo (\* 2 (- 10 5)), com resultado 10. Comandos foram agregados com o passar do tempo para manter a linguagem popular e aumentar sua eficiência, mas mesmo assim, como já dito, a mesma não se conquistou uma grande popularidade no mercado devido às limitações em termos de aplicações práticas desejadas pelo mercado provavelmente.

Uma linguagem implementada recentemente pela JetBrains é chamada kotlin e propõe uma programação eficiente no desenvolvimento para web, mobile e desktop. Esta linguagem possui como base a orientação a objetos, mas por permitir que funções sejam escritas fora de classes, pode implementar códigos puramente funcionais como em linguagens baseadas no paradigma funcional.

Fonte:[Disponível aqui](https://kotlinlang.org/docs/kotlin-docs.pdf)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

## Linguagem Scheme

A linguagem Scheme, criada na década de 1970, foi desenvolvida com base na linguagem Lisp e trata funções de maneira um pouco diferente, podendo ser valores de expressões ou elementos de listas, e assim, podendo ser utilizadas como dados para variáveis ou parâmetros, recurso que não era oferecido pela versão original de Lisp segundo Sebesta (2011).

Sendo uma linguagem simples, de fácil compreensão de sua sintaxe e semântica, funciona como boa opção para uso educacional, e seu interpretador que interage com o usuário permite que diferentes solicitações sejam feitas e avaliadas em tempo de execução.

Como em Lisp, expressões são escritas entre parênteses que funcionam como delimitadores e como elementos de controle da precedência das operações realizadas nas funções.

| Expressão | Resultado |
| --- | --- |
| 10 | **10** |
| (+) | 0 |
| (\*) | 1 |
| (+ 2 2) | 4 |
| (- 5 3) | 2 |
| (\* 2 (+ 1 3)) | 8 |
| (/ 3 (+ 4 5)) | 3 |

Fonte: O autor.

Nos exemplos da imagem, o primeiro informa ao interpretador apenas um elemento primitivo e o mesmo é retornado como resultado, mas nos segundo e terceiro exemplos, como as expressões são escritas tendo apenas o operador sem elementos de parâmetros, os resultados são 0 e 1, respectivamente os elementos neutros de cada operação.

Na sequência, os demais exemplos trazem expressões completas utilizando apenas átomos ou expressões compostas de átomos e outras expressões com operações primitivas, as regras de precedência são aplicadas e os cálculos realizados, retornando os valores expostos ao lado das expressões.

Existem diversas linguagens de programação utilizando o paradigma funcional para poderem implementar a função lambda e outros recursos, e linguagens como Java a partir de sua oitava versão e Python, possuem além dos paradigmas orientado a objeto, o paradigma funcional agregado.

Python é uma linguagem que utiliza muito mais naturalmente o multiparadigma orientação a objetos e funcional em uma sintaxe limpa e que facilita interpretação e manutenção de código, mesmo misturando paradigmas.

**def par (x):**

**return (x % 2) == 0**

Fonte: Acesse o link [Disponível aqui](https://docs.python.org/pt-br/3/howto/functional.html)

Neste código, é fácil imaginar uma linguagem tipicamente funcional pelas características sintáticas presentes, mas é um código completo e funcional em linguagem Python pelo paradigma funcional existente.

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

A semântica básica da linguagem Scheme se baseia em definições de funções, e escrevê-las corretamente é o que deve ser primeiramente compreendido para que se possam gerar aplicações para esta linguagem.

Um detalhe curioso é que o código pode ser escrito de forma que o usuário interaja com o mesmo a partir do prompt do interpretador, ou pode ser incluído no código, expressões a serem executadas logo que o código tenha sido executado e como próximo passo, estaria aguardando interação.

**(define dobro**

**(lambda (x)**

**(\* 2 x)))**

**(dobro 5)**

Fonte: autor.

No exemplo da figura, temos a definição de uma função chamada dobro() usando a função primitiva **define** que associa uma função lambda() que aplica num valor recebido para x, o cálculo que realiza a multiplicação por 2. Após a definição da função dobro(), é inserida uma linha de comando que já atribui o valor 5 como parâmetro para a função dobro() permitindo assim que a aplicação já possa executar diretamente o cálculo para este valor.

A sintaxe da linguagem Scheme para ações comuns como entrada e saída de dados é bastante simples e é baseada também na construção de expressões como funções delimitadas por parênteses.

| **CÓDIGO** | **EXECUÇÃO** |
| --- | --- |
| **(display "Digite um valor: ")**  **(define x (read))**  **(display "X ao quadrado: ")**  **(display (\* x x))**  **(newline)**  **(display "X ao cubo: ")**  **(display (\* x x x))**  **(newline)** | **Digite um valor: 3**  **X ao quadrado: 9**  **X ao cubo: 27** |

Fonte: O autor.

Pelo exemplo da imagem, é possível observar a forma como se estrutura código contendo entrada de dados através da função (*read*) inserida em outra função que usa a palavra reservada define para atribuir o retorno da função de leitura de dados a uma variável x.

Também são utilizadas funções (*display*) para exibir mensagem a usuários, sendo padronizados os conteúdos para exibição como texto delimitado por aspas, ou expressões construídas entre parênteses.

Por fim, para que a execução tenha uma aparência mais agradável, e tanto a mensagem que traz uma explicação do valor do cálculo do quadrado do valor de x, quanto do cubo de x sejam exibidas de forma a facilitar a leitura e interpretação, após a exibição do resultado de cada função, a função (*newline*) se encarrega de mudar de linha na tela de exibição.

Por esses exemplos das imagens já apresentadas nesta aula, fica nítida a construção de códigos em forma de funções delimitadas sempre por parênteses, mostrando a simplicidade sintática do paradigma e da linguagem, além de uma manutenção mais fácil de código se necessário.

Um dos fundamentos da programação funcional que é o uso de funções serve também de base para um dos conceitos mais importantes da programação, a recursão.

Na figura a seguir, temos um exemplo clássico de cálculo de fatorial que utiliza o mecanismo de recursividade para realizar sucessivas iterações e retornar ao final destas o valor calculado desejado.

**(define (fat n)**

**(if (= n 0)**

**1**

**(\* n (fat (- n 1)))))**

Fonte: autor.

A recursão no paradigma funcional da linguagem Scheme não se diferencia muito do recurso em uma linguagem imperativa, por exemplo, e a premissa de que a função recursiva deve ser composta por uma estrutura de decisão onde a condição representa um critério de parada, e enquanto esta condição não for satisfeita, a função chama a si mesma de forma que a cada iteração ela caminhe na direção de atender à condição de parada é o mesmo.

A linguagem Haskell é mais um exemplo de linguagem funcional, mas pura, similar à linguagem ML, mas com diferenças sintáticas importantes, pois a linguagem ML possui uma construção de códigos mais semelhante às demais linguagens utilizadas nesta aula, mas Haskell possui uma sintaxe mais parecida com a escrita de sistemas de equações matemáticas.

Imagem 47

| **ML** | **Haskell** |
| --- | --- |
| fun fact(n: int): int = if n = 0 then 1 else n \* fact(n - 1); | fact 0 = 1  fact n = n \* fact (n – 1) |

Fonte: Adaptado de Sebesta, 2011.

É intuitiva a análise dos dois códigos presentas na imagem 47, pois ambos possuem uma função chamada fact(), uma condição de parada associada ao valor 0, e chamadas recursivas à própria função com redução do valor da variável n utilizada como parâmetro de entrada.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Linguagem Lisp
- Linguagem Scheme

Para complementar seus estudos, assista à videoaula a seguir: