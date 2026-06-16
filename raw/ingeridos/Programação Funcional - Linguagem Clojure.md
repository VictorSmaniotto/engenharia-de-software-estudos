---
title: "Aula 11 - Programação Funcional - Linguagem Clojure"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-11.html"
author:
published:
created: 2026-05-19
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 11 - Programação Funcional - Linguagem Clojure

Uma opção de linguagem que pode exemplificar a programação funcional é a linguagem Clojure, fruto de uma seleção de aspectos de várias outras linguagens como Ruby, Python, Java e Haskell para oferecer soluções a problemas enfrentados por desenvolvedores destas linguagens.

## Linguagem Clojure

Linguagem interpretada que funciona com base na máquina virtual Java (JVM), pode se utilizar de bibliotecas Java, que por si só já lhe confere uma extensa gama de facilidades, permitindo inclusive que aplicações Clojure e Java sejam empacotadas juntas.

Por ser baseada em Lisp, possui características boas da linguagem que permitem que tenha desempenho até superior a outras linguagens como Java e Python que possuem origem baseada em C e Algol.

Por ser uma linguagem funcional, trabalha com conjuntos de dados imutáveis (átomos) e funções primárias, redução de problemas com um controle forte de mudanças de estados, permitindo o desenvolvimento de soluções que utilizem os mecanismos de concorrência e paralelismo.

Para isso, permite que se desenvolvam aplicações utilizando tecnologias de hardwares como de múltiplas CPUs e múltiplos núcleos e computação distribuída, segundo Emerick (2012) que necessitam de linguagens de programação que possuam mecanismos para suportar estas tecnologias.

Outro mecanismo interessante da linguagem Clojure é que ela permite carregamento de código em tempo de execução, sendo importante em aplicações de missão crítica que necessitam estar no ar o tempo todos e assim, permitindo atualizações para correção ou melhorias sem interrupção dos serviços.

A forma como são elaborados os códigos no paradigma funcional é bastante diferente dos demais e inicialmente é bem complexa sua lógica e consequentemente, seu aprendizado, mas com o tempo, a simplicidade dos códigos de programação funcional vão sendo assimilados e a qualidade de ser necessária uma menor quantidade de código em relação a linguagens imperativas ou orientadas a objetos para as mesmas funcionalidades se torna uma vantagem.

No exemplo da figura a seguir, é possível observar um pequeno código que seria maior em praticamente qualquer linguagem em paradigmas estruturado ou orientado o objeto devido ao fato de lidar com lista de valores e funções.

```clojure
(defn media

\[numeros\]

(/ (apply + numeros) (count numeros))

)
```

Fonte: autor.

Nele, uma função media é definida com o uso da função primitiva defn que recebe uma lista de números entre colchetes. A função possui a função primária apply realizando a soma dos números informados e a outra função primária contando a quantidade de elementos do conjunto fornecido.

Assim, pela utilização de uma função de soma dos valores dos elementos e outra de contagem de elementos passados como parâmetros, é possível aplicar a última função primitiva de divisão do resultado da função de soma pelo resultado da função de contagem, obtendo-se então a média aritmética dos valores recebidos como parâmetros pela função media.

Os códigos foram utilizados no ambiente online para teste de programação em diversas linguagens chamado de REPL.IT (https://repl.it) que será utilizado como padrão para teste dos exemplos desta e de outras linguagens de programação ao longo do material como já citado.

```clojure
(def agenda {:nome "Fulano de Tal"

:fone "3322-5566"})

(:nome agenda)

" Fulano de Tal"
```

Fonte: autor.

Outro exemplo de código é mostrado na imagem acima, na utilização da função primitiva *def* para que uma estrutura de dados chamada agenda possa receber dados indicados por rótulos **:nome** e **:fone**, que sendo referenciados durante a execução, retornam o dado relacionado ao rótulo informado (nome neste caso).

Nessa situação da imagem acima, uma diferença importante fica por conta da delimitação dos dados rotulados com o uso de chaves, ao invés da lista de elementos delimitados por colchetes na imagem anterior.

Colocando apenas o nome de uma função que necessita de parâmetros não traz resultado algum. Inserir os parâmetros após o nome da função simplesmente como poderia ser feito em outras IDEs e com algumas outras linguagens funcionaria. Inserir os parâmetros corretamente em forma de lista para a soma está correto, mas sem o uso dos parênteses que caracterizam funções no paradigma também geram erros de sintaxe.

Como já citado, a forma como são estruturadas as expressões em programação funcional também são diferentes, pois seguem a chamada notação polonesa ou prefixa onde os operadores são colocados antes dos operandos (valores) na ordem em que devem ser utilizados, e aparentemente é uma notação mais confusa que a tradicional infixa que todos estão acostumados onde os operadores ficam intercalados com os valores.

Um exemplo simples seria a soma 3 + 4 utilizada nas linguagens de paradigmas estruturados e orientados a objeto, por exemplo, e em notação prefixa ficaria + 3 4 que é a forma padrão do paradigma funcional.

Alguns operadores também são escritos de forma diferente em Clojure em relação a C, por exemplo. O operador para negação! é substituída pelo operador *not*, o operador ++ antes de uma variável é substituído pelo operador *inc*, etc.

Como toda a semântica da linguagem é pensada em funções e notação prefixa, a elaboração de códigos tende a ser mais complexa por não ser algo natural do ser humano esta forma de elaboração de pensamento, mas com o tempo e prática de códigos diversos para compreender todo o conceito de uma linguagem funcional, é possível que sejam produzidos códigos muito bons e altamente eficientes.

```clojure
(defn hypot
\[x y\]
(let \[x2 (\* x x)
y2 (\* y y)\]
(Math/sqrt (+ x2 y2))
)
)
```

Fonte: Sebesta (2011).

O código da imagem traz uma aplicação de cálculo da hipotenusa em um triângulo, que representa o maior lado, baseado nos valores dos catetos que estão representados pelos dois lados restantes do triângulo.

Para isto são declaradas duas variáveis x2 e y2 que recebem os valores de x e y respectivamente através da função primitiva *let* que permite que as funções contidas dentro dos colchetes sejam processadas e os valores de x sejam elevados ao quadrado, assim como o valor de y, de acordo com a fórmula trigonométrica.

Uma excelente maneira de se conhecer as qualidades da programação funcional é através do estudo de uma linguagem que lhe permita utilizar o que se conhece e agregar o novo paradigma.

A linguagem JavaScript é uma boa alternativa, pois é muito utilizada no mercado (fato que pode render um emprego rápido) e aceita o desenvolvimento de códigos com ou sem o uso do paradigma funcional, permitindo uma migração mais tranquila.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

A sintaxe das linguagens funcionais é muito similar a matemática e por mais que não haja uma variação muito grande na sintaxe para construção de funções, a lógica utilizada nestas construções pode ser bastante complexa e unir grande quantidade de símbolos e ações não convencionais em linguagens imperativas, por exemplo.

Imagem 39

| **CÓDIGO** | **EXECUÇÃO** |
| --- | --- |
| **(defn doubler**  **\[f\]**  **(fn \[& args\]**  **(\* 2 (apply f args)))**  **)** | **\>>> (def double-+ (doubler +))**  **\>>> (double-+ 1 2 3)**  **\>>> 12** |

Fonte: Adaptado de Sebesta (2011).

No exemplo da imagem 39 é mostrado uma forma muito diferente de execução de uma aplicação onde o código traz uma forma aberta de definição de função doubler() onde & *args* permite que seja definida uma função double() inclusa dentro de doubler(), e que aplica a multiplicação por 2 sobre a expressão definida pela chamada da função double() definida em tempo de execução.

Na coluna da esquerda, o código possui apenas a função doubler() que está completa, mas deixa em aberto a definição de uma função que será realizada, sendo então definida durante a execução por (def double-+ (doubler +)).

Depois a chamada da função double() com a operação soma indicada para os três valores passados como parâmetros de entrada, realiza a soma dos três e depois o resultado é aplicado na multiplicação da função principal doubler().

Para ter uma ideia de uma aplicação um pouco maior utilizando o paradigma funcional, um exemplo que é muito comum de ser implementado no estudo da programação em si é uma calculadora, pois ajuda a conhecer operações e expressões, funções e estruturas de decisão num mesmo código, oferecendo bom nível de treino e aprendizado.

| **CÓDIGO** | **EXECUÇÃO** |
| --- | --- |
| **(defn soma \[a c\]**  **(+ a c))**  **(defn sub \[a c\]**  **(- a c))**  **(defn mult \[a c\]**  **(\* a c))**  **(defn div \[a c\]**  **(/ a c))**  **(defn calc**  **\[a b c\]**  **(cond**  **(= b +) (soma a c)**  **(= b -) (sub a c)**  **(= b \*) (mult a c)**  **(= b /) (div a c)**  **)**  **)** | **\>>> (calc 4 + 2)**  **\>>> 6**  **\>>> (calc 8 \* 3)**  **\>>> 24**  **\>>> (calc 2 - 3)**  **\>>> -1**  **\>>> (calc 4 / 2)**  **\>>> 2**  **\>>> (calc 7 / 2)**  **\>>> 7/2**  **\>>> (calc 3 / 0)**  **\>>> Divide by zero!!!** |

Fonte: O autor.

No código da imagem é clara a ideia da codificação em funções, pois são definidas funções para cada diferente cálculo (soma, *subt*, *mult* e *div*) e uma função calculadora para conter as instruções essenciais da função de chamada do programa e que pode acessar as demais funções declaradas.

Neste exemplo foram testados alguns cálculos, e um ponto curioso é que foram solicitadas três divisões para mostrar o que ocorre com variadas situações, mostrando a importância de serem realizados testes com aplicações.

Na primeira divisão, temos o resultado 2 para uma divisão exata, mas no segundo, a fração 7/2 é retornada como resultado por se tratar de uma operação com resultado de ponto flutuante com casas decimais, e por fim, no terceiro teste, uma convenção básica da matemática é ferida e ocorre um erro na tentativa de divisão de um número qualquer por zero que é uma operação indefinida.

Os conceitos e exemplos desta linguagem servem como ilustração de alguns dos conceitos de uma linguagem funcional, mas em caso de interesse, existe muito material adicional que pode ser explorado sobre a linguagem Clojure.

A linguagem Clojure, por conseguir comunicar-se com bibliotecas Java, sendo este um excelente argumento de uso, mas ainda existem variações da linguagem como Clojure CLR para conversão de código e adaptação para plataformas.NET ou ClojureScript que converte códigos da linguagem para JavaScript.

Cerca de 90% dos micro serviços utilizados pela Nubank estão escritos em Clojure, e diversas bibliotecas foram desenvolvidas pela própria equipe de desenvolvimento da empresa para agilizar o desenvolvimento de aplicações onde se pudesse reaproveitar código.

Acesse o link:[Disponível aqui](https://blog.nubank.com.br/o-que-e-clojure/)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Linguagem Clojure

Para complementar seus estudos, assista à videoaula a seguir: