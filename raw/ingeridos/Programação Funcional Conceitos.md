---
title: "Aula 10 - Programação Funcional Conceitos"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-10.html"
author:
published:
created: 2026-05-19
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 10 - Programação Funcional Conceitos

O chamado paradigma funcional possui um viés mais matemático e permite uma forma mais específica de desenvolvimento de código onde toda a codificação se baseia no conceito utilizado em funções matemáticas e representa um importante paradigma não imperativo de programação.

Linguagens como Lisp, ML, Scheme e Haskell se baseiam neste paradigma para a estruturação de sua semântica e sintaxe inicialmente, mas podendo adicionar conceitos de outros paradigmas para que pudessem se tornar linguagens mais versáteis.

## Funções

Matematicamente, uma função representa uma relação entre elementos numéricos de um conjunto chamado **domínio** e outro chamado **imagem**, partindo de alguma operação ou expressão aplicada nos elementos do domínio, que resultam sempre em elementos do conjunto imagem. Observe a imagem a seguir para compreender o conceito de forma gráfica.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a10-figura1.svg)

Fonte: O autor.

No exemplo, é exibida uma representação gráfica genérica com base do chamado diagrama de Venn que usa círculos para representar conjuntos e setas representando as relações entre os elementos de cada conjunto, sendo que a origem da seta ocorre em um elemento do conjunto domínio, e a seta aponta para um elemento do conjunto imagem.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a10-figura2.svg)

Fonte: O autor.

Um exemplo prático de função matemática é mostrado na imagem acima, em que é possível observar que a aplicação de determinada operação sobre os elementos do conjunto domínio A, resultam nos elementos de um conjunto imagem B, e a operação neste exemplo seria a de multiplicar os elementos de A por 2.

No caso da programação, geralmente as funções recebem parâmetros de entrada e os processamentos são realizados com base neste parâmetro ou a função não recebe parâmetros, mas pode manipular dados de fora dela.

Um ponto importante é a forma como os parâmetros podem ser definidos, havendo diferenças entre as implementações das linguagens que podem aceitar apenas variáveis declaradas com tipos primitivos, podem aceitar estruturas de dados mais complexas, ou até objetos e estruturas inteiras.

De forma similar às sintaxes de programação em geral, uma função é escrita iniciando-se pelo identificador da mesma, seguido por um dado, variável ou expressão entre parênteses, funcionando como os parâmetros em programação e depois, a forma como os dados de parâmetros são processados.

A execução do código em linguagens deste tipo ocorre na ordem definida para as operações, tendo regras definidas e não executadas da forma sequencial como ocorre na programação imperativa.

As chamadas funções puras possuem uma característica importante que se chama imutabilidade que define que uma função, ao receber um parâmetro e utilizar seu valor no processamento interno, sempre deve retornar o mesmo resultado. Uma função que recebe um valor multiplica esse valor por ele mesmo e retorna este resultado obtido é imutável, pois sempre que um valor for passado como parâmetro, o mesmo resultado do valor ao quadrado será retornado, ao passo que numa função de receba um valor e utiliza um dado presente em uma variável externa à função para uso em cálculos, se torna impura, dependendo do valor desta variável para determinação do resultado. O cálculo da cotação de uma moeda que recebe de fora da função o valor para conversão, sem que este seja recebido como parâmetro torna a função impura e assim, menos confiável em relação a não ocorrência de exceções. Funções imutáveis são excelentes no processo de teste e implantação de softwares, pois existe uma confiança de que os resultados são realmente previsíveis e as chances de exceções reduzidas.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Em Lisp, dois tipos de dados básicos são utilizados apenas, chamados de átomos e listas, e estes átomos representam tanto dados numéricos, quando alfanuméricos (caracteres).

As listas são declaradas entre parênteses e representam conjuntos de átomos ou outras listas que também usam parênteses para definir seus próprios elementos. Um exemplo de lista contendo átomos e uma lista poderia ser representado por (1 2 3 (4 5) 6), sendo que 1, 2, 3 e 6 são átomos contidos na lista, e (4 5) representa uma lista contida dentro desta outra lista maior. Pode-se dizer então que a lista possui 4 átomos e uma lista, mas de forma geral, possui 5 elementos componentes.

Neste paradigma, os tipos de dados são um diferencial e como não é um paradigma de propósito geral, sendo pensado em aplicações dentro de um escopo reduzido, não são necessários muitos tipos diferentes e complexos, sendo este ponto, um elemento que simplifica o aprendizado de linguagens de programação funcionais.

Geralmente, as funções são escritas de forma simples com sintaxes bem intuitivas e de fácil interpretação, onde a operação ou função propriamente dita pode ser indicada como primeiro elemento da lista, seguido dos átomos a serem utilizados na função. Esta notação pré-fixada (também conhecida como notação polonesa) é utilizada em calculadoras financeiras, por exemplo.

Na década de 1940, Alonzo Church definiu o termo **lambda** para funções não nomeadas, conceito que foi adotado pelo paradigma e um dos conceitos que é adotado em linguagens de programação que agregam este paradigma ao(s) já existentes como fez a linguagem Java em sua versão 8.

As funções definidas neste paradigma devem ser de natureza pura, ou seja, se um determinado dado for utilizado como parâmetro de entrada para ser utilizado nos processos internos de uma função, esta deve retornar sempre o mesmo resultado, evitando assim, efeitos colaterais indesejáveis causados por resultados não esperados.

Para uma função ser pura e gerar sempre um mesmo resultado, é preciso garantir que isto ocorra, e um dos motivos de modificação e resultado da uma função é o uso de dados de fora da função que não sejam adquiridos através dos parâmetros de entrada, como no uso de dados de variáveis globais em uma função, pois estes podem ser alterados a cada execução e os retornos de uma função para os mesmos parâmetros de entrada poderiam ser diferentes.

Esse problema pode ser resolvido pelo não uso de dados externos além dos recebidos por parâmetros e isto é facilmente resolvido apenas adicionando o valor da variável global como parâmetro da função, e por garantia, se possível, mudar a variável para local de forma que sempre que precise ser utilizada ou ter seu dado atualizado, isto seja feito por passagens de parâmetros e atribuições de dados vinculados a retornos de funções, como uma alternativa de solução.

Conceitos comumente utilizados em outros paradigmas podem ferir o fundamento de pureza de uma função, como na passagem de arquivos como parâmetros, pois podem ter seu conteúdo alterado, e assim, podendo gerar mudanças no retorno da função, assim como funções que utilizam números aleatórios em seu processamento, tendo assim também, a possibilidade de geração de diferentes retornos com um mesmo dado utilizado como parâmetro de entrada.

Os efeitos colaterais estão ligados a ações que uma função pode realizar e que não sejam totalmente previsíveis ou seguras como alterações de valores em estruturas de dados fora da função que não dependam de aguardar o retorno de dados ao final da execução da mesma, ou seja, atribuições de valores em variáveis ou outras estruturas de escopo global pela função.

O uso de funções puras traz benefícios para desenvolvedores, pois são mais previsíveis em função do maior controle dos dados e processos, mais estáveis e robustos, além de simplificarem a leitura do código e sua compreensão.

Uma função sendo pura favorece seu teste, seu reuso e sua integração, pois se sabe que uma função assim é mais facilmente testável e manipulável, facilitando a compreensão do código.

O conceito de linguagem funcional pura, segundo Sebesta (2011), não utiliza variáveis e nem instruções de atribuição de dados, reduzindo preocupações com recursos de hardware, mas sem a disponibilidade de variáveis, não se pode gerar laços de repetição, pois são controlados justamente por variáveis para atualização do número de iterações e a recursividade é uma solução à ausência de estruturas de repetição.

As linguagens funcionais mais gerais agregam recursos como o uso de variáveis e acabam gerando mudanças de estado e outros recursos que aumentam a versatilidade destas linguagens, mas consomem mais recursos de hardware e possuem menor desempenho em relação a uma linguagem funcional pura. Um aspecto que pesa no desempenho é a recursão que é mais lenta que a estrutura de repetição equivalente, mas existem compiladores que convertem recursões em estruturas iterativas para reduzir este mecanismo mais lento sem que o código necessite ser escrito de outra forma ou outra linguagem.

Linguagens funcionais possuem funções primitivas, mecanismos para a construção de funções complexas a partir de funções primitivas, e formas de representação de dados para parâmetros e retornos destas funções.

Quando se une uma linguagem funcional com uma imperativa, por exemplo, gerando uma linguagem multiparadigma, existem recursos que precisam ser analisados como o caso de uma linguagem imperativa permitir retornos de tipos mais limitados geralmente, como tipos primitivos, e isto limita o potencial do paradigma funcional.

A programação funcional possui forte referência matemática, mas pode ser aplicada no desenvolvimento de soluções para outros fins. O importante é que as características deste paradigma possam oferecer meios de se desenvolver software mais eficiente para determinados tipos de soluções computacionais.

> Isso significa que, no paradigma funcional, você tem uma função, coloca um dado de entrada, aplica várias operações e obtém uma saída. É possível alterar as operações e, consequentemente, a saída, mas a entrada sempre permanecerá a mesma.

Os códigos em programação funcional tendem a ter menos linhas, sendo uma alternativa de linguagem que tende a ser mais fácil de manter e evoluir códigos, testar e avaliar falhas.

Fonte:[Disponível aqui](https://blog.nubank.com.br/programacao-funcional-o-que-e-relacao-nubank/)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Funções

Para complementar seus estudos, assista à videoaula a seguir: