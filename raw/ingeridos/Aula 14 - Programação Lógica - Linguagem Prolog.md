---
title: "Aula 14 - Programação Lógica - Linguagem Prolog"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-14.html"
author:
published:
created: 2026-06-18
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 14 - Programação Lógica - Linguagem Prolog

A linguagem Prolog trabalha com o conceito de declarações de fatos sobre objetos que servem para a estruturação de relacionamentos ou regras entre fatos de objetos e objetos em si. Utiliza, além de fatos e regras, a possibilidade de uso de variáveis e listas de dados, além da possibilidade de implementação de recursividade.

## Linguagem Prolog

Diferentemente da programação imperativa e estruturada em que algoritmos se baseiam na manipulação de dados, no paradigma lógico, a proposta é de se pensar em o que serve de base para processamento ao invés de como devem ser processados os dados.

As chamadas proposições atômicas são formadas por relações que possuem uma sintaxe não muito diferente da programação funcional, e as relações incidem sobre termos (átomos em Lisp) inseridos em listas indicadas entre parênteses e separados por vírgulas.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a14-figura1.svg)

Fonte: O autor.

No exemplo da imagem, existem 4 fatos determinados pelas proposições indicadas que servem de base para os fatos da relação amigo, e esta pode ser ilustrada como diagrama apenas para que fique clara a ideia de quem é amigo() de quem pela ordem dos elementos.

No código, a relação amigo() é aplicada aos termos ana, marcos, silvio, paulo e victor, sendo cada linha chamada de instância. As instâncias são aplicações diretas de relações sobre listas de termos, e o conjunto de instâncias representa a relação em si.

Esta diferenciação de ordem na relação amigo() pode não ser relevante, pois esta relação possui a propriedade comutativa, ou seja, se for escrito amigo(ana, marcos) ou amigo(marcos, ana) a relação terá o mesmo resultado e significado pela relação ser assim.

Se fosse outra relação como altura, idade ou cargo em uma hierarquia, seria diferente e, por exemplo, uma relação chefe(ana, marcos) não poderia ter o mesmo valor lógico de chefe(marcos, ana), pois uma poderia ser verdadeira, mas daí, certamente a outra não poderia ser, pois a relação chefia não é comutativa.

Em relações não comutativas como a usada no exemplo chefe(), poderiam ser utilizadas setas para indicar no diagrama, a ordem dos termos que representariam a correta aplicação da relação entre os elementos.

O problema é que na programação, a linguagem não interpreta o sentido do nome da relação, e para o interpretador, a relação se chamar amigo(), chefe() ou abc() não faz diferença, pois o que vale são as definições de instância para que a relação seja definida.

Para esta linguagem, pode ser usada a plataforma https://swish.swi-prolog.org/ para execução dos códigos em linguagem Prolog, sendo uma plataforma online para interpretação e teste de códigos.

Para verificar se a relação está corretamente definida por suas instâncias, pode-se testar a mesma utilizando comandos a serem interpretados durante a execução que podem verificar se o código foi corretamente escrito e a relação definida de maneira precisa.

Imagem 1

**? amigo(X, Y).**

X = ana,

Y = marcos

X = ana,

Y = silvio

X = paulo,

Y = victor

X = victor,

Y = marcos

Imagem 2

**? amigo(marcos, Y).**

false

Com esses dois testes colocados na imagem, temos a indicação de que algo não está correto, pois se solicitamos que todas as instâncias sejam exibidas indicando variáveis em aberto X e Y para a relação, qualquer termo das instâncias é aceito e todas as instâncias definidas aparecem na tela.

No segundo teste, o resultado acusa falso para amigos de marcos, mas isto não deveria ocorrer, pois **marcos** é amigo de **ana** e **victor**. Isto ocorreu porque nas instâncias, marcos está como segundo termo da relação na instância e no comando de teste, foi colocado como primeiro.

Como o interpretador não “imagina” que a relação possa ser comutativa, simplesmente não encontra instâncias onde marcos esteja à esquerda em conjunto com qualquer outro termo pertencente às instâncias da relação.

Para que a relação entenda a comutatividade e o lado que for referenciado para a busca por amigos se torne irrelevante, como deve ser, é possível ensinar ao interpretador que a ordem inversa dos termos também representa uma mesma relação, e para isto, é preciso adicionar as relações invertidas indicadas nas relações já definidas.

Imagem 3

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a14-figura2.svg)

Adicionando instâncias com a ordem dos termos invertidos à relação anterior da imagem 1, a nova relação mostrada na imagem 3 agora está com a comutatividade representada, e assim, representando as possibilidades de amizades corretamente.

Com isto, um novo teste com a nova relação, utilizando o mesmo comando que resultou falso no exemplo da imagem 2, agora deve retornar o resultado que aparece na imagem a seguir.

Imagem 4

**? amigo(marcos, Y).**

Y = ana

Y = victor

Prolog utiliza termos definidos por constantes que possuem nomes que iniciam por letras minúsculas ou variáveis definidas por nomes que iniciam por letras maiúsculas, ou outras estruturas que representem relações.

As relações podem ser definidas em sequência no código, montando uma base mais complexa de fatos e relações que podem oferecer resultados mais interessantes à medida que a lista de instâncias aumenta, variando as relações e estas, vão tendo ligações entre si.

Um dos exemplos clássicos para demonstração de Prolog se aplica ao conceito de árvore genealógica e para exemplificar como uma linguagem deste tipo pode organizar uma estrutura assim, observe o exemplo da imagem 5.

Imagem 5

pai(joao, pedro).

pai(joao, ana).

mae(maria, pedro).

mae(maria, ana).

irmãos(pedro, ana).

irmãos(ana, pedro).

Fonte: autor.

Partindo das instâncias definidas nestas relações da imagem 5, existe uma mescla entre relações comutativas e não comutativas onde irmãos() é uma relação comutativa e pai() e mae() são relações não comutativas, onde não se pode inverter os termos das instâncias para mantê-las como verdadeiras.

O melhor caminho para se aprender a elaborar relações é tentar imaginar problemas que necessitem que dados sejam relacionados entre si, como ocorrem em bancos de dados, e implementar instâncias que simulem as relações entre dados. Observar depois se as relações foram corretamente definidas por um conjunto adequado de instâncias informadas e testar todas as possibilidades de forma a encontrar falhas na definição das relações como foi visto em relações comutativas onde as duas possibilidades de instância com os mesmos termos não é definida.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Imagem 6

**? pai(joao, X).**

X = pedro

X = ana

**? mae(maria, Y).**

Y = pedro

Y = ana

**? irmãos(Z, W).**

W = ana,

Z = pedro

W = pedro,

Z = ana

Como é possível conferir pelos resultados exibidos na imagem 6, as relações estão definidas a partir das instâncias, e os irmão aparecem duas vezes como resultados em função da comutatividade.

Também é possível realizar processamento de dados em tempo de execução e expressões podem ser calculadas com dados contidos nas instâncias, por exemplo. Observe o exemplo da imagem 7.

Imagem 7

**% pessoa(Nome, Horas trabalhadas, Salário)**

**pessoa(jair, 160, 2000).**

**pessoa(paulo, 150, 3000).**

**pessoa(felipe, 172, 2500).**

No exemplo da imagem 7, é fornecida uma base de dados pessoais em três instâncias que definem a relação pessoa. Nestas três instâncias, são fornecidos termos em forma de texto e número para que se obtenha uma pequena base de dados heterogêneos.

Com base nos dados contidos nos fatos apresentados, alguns novos dados podem ser obtidos a partir da aplicação de cálculos realizados sobre os dados presentes nos termos das instâncias.

Imagem 8

**? pessoa(X,Y, Z), Media is Z/Y.**

Media = 12.5,

X = jair,

Y = 160,

Z = 2000

Media = 20,

X = paulo,

Y = 150,

Z = 3000

Media = 14.534883720930232,

X = felipe,

Y = 172,

Z = 2500

Neste exemplo da imagem 8, utiliza-se no momento da execução uma solicitação que utiliza os termos como base para se realizar um cálculo para descobrir a média salarial por hora de cada pessoa, associando a divisão do salário pela quantidade de horas trabalhadas, armazenando-as num novo termo chamado Media.

A linguagem Prolog, assim como as demais citadas até aqui, possui diversas outras funcionalidades que podem ser exploradas com estudos mais aprofundados. Para os estudos deste material, apenas alguns aspectos são trazidos de forma a apresentar algumas das diversas linguagens de programação existentes no mercado.

A linguagem Prolog mostra-se bastante diferente na construção de soluções computacionais, mas como toda linguagem, pode ser utilizada na solução de determinados tipos de problemas geralmente.

Algumas aplicações que podem trabalhadas com a linguagem Prolog são nas áreas de computação simbólica como prova automática de teoremas, bancos de dados relacionais, linguagem natural, solucionadores de jogos e sistemas especialistas, dentre outros.

Fonte:[Disponível aqui](http://ww2.inf.ufg.br/~eduardo/lp/alunos/prolog/prolog.html)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

Fonte: Freepik.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a14-img03.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Linguagem Prolog

Para complementar seus estudos, assista à videoaula a seguir: