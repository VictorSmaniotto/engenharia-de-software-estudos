---
title: "Conceitos Gerais de Programação"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-01.html"
author:
published:
created: 2026-05-07
description:
tags:
  - "clippings"
---
Conceitos Gerais de Programação

Disciplina: Algoritmos e Lógica de Programação
Aula 01 - Conceitos Gerais de Programação

Sumário[1\. Formas de representação de soluções de problemas](#topico-01)[

2\. Estrutura de um algoritmo

](#topico-02)[

3\. Palavras reservadas

](#topico-03)

Programar é um ato que depende não só das habilidades de um profissional de desenvolvimento de *software* ou uma equipe de desenvolvedores, pois a complexidade dos problemas a serem resolvidos varia de pequenos componentes de um *software* a problemas computacionais complexos ou o desenvolvimento de grandes sistemas inteiros.

Isso faz com que sejam necessários outros profissionais, além de programadores, para que se possa compreender o problema a ser resolvido e a estruturar uma solução a ser desenvolvida a partir de requisitos identificados no problema, com prazo e orçamento disponíveis, pois estes dois últimos aspectos também afetam muito as decisões de como pode ser produzido um *software* para o que é pedido pelo cliente e se é possível produzi-lo de forma aceitável.

Uma das etapas do desenvolvimento de uma solução computacional pode talvez ser a mais importante, pois é nela que a solução propriamente dita é elaborada já com um olhar computacional, e esta etapa pode ser uma etapa real do processo de desenvolvimento ou algo já tão desenvolvido que pode ser praticamente pensado automático e instantaneamente paralelo ao desenvolvimento de um código em determinada linguagem de programação.

Este desenvolvimento de uma solução intermediária entre a modelagem inicial de uma solução computacional e seu desenvolvimento de código propriamente dito, chamado de algoritmo, simboliza representações em idioma local de uma possível solução computacional, mais visando a compreensão lógica de uma solução proposta e dos mecanismos de programação que podem ser utilizados na solução.

Independentemente da forma como será elaborada uma solução, o mais importante nesta etapa do aprendizado do desenvolvimento de *software* é a lógica utilizada para solucionar problemas e compreender a estrutura de um código, lembrando que existem diferentes formas de se estruturar códigos devido a diferenças que existem nos chamados paradigmas que as linguagens de programação podem utilizar em suas implementações, além das diferenças de sintaxe na construção de instruções.

Os paradigmas se referem a diferentes formas de se programar como na programação estruturada ou orientada a objetos, por exemplo, e a chamada sintaxe se refere a como cada instrução é implementada em cada linguagem, pois em algumas há muitas semelhanças, mas em outras, a sintaxe varia muito em função da diferença de paradigma e da forma como foi implementada a linguagem.

## Formas de representação de soluções de problemas

Além do uso de algoritmos, é possível representar possíveis soluções computacionais de problemas utilizando narrativas em idioma local em forma de frases curtas contendo todos os principais processos que ocorrem na execução da solução. Observe um exemplo de descrição narrativa na imagem 1.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a01-fig01.svg)

Imagem 1: Exemplo de narração descritiva | Fonte: O autor.

Neste exemplo da imagem 1, a descrição narrativa traz uma alternativa de solução para a identificação de valores positivos ou negativos que podem ser inseridos como entradas de dados em uma solução computacional. Nesta alternativa é possível perceber o uso de frases curtas em idioma local que são facilmente compreendidas por pessoas, mas não representa exemplo de código em linguagem de programação *software* propriamente dito.

Outra forma de solução utiliza um diagrama bastante específico chamado de fluxograma que tem por função essencial, demonstrar a sequência de ações que ocorre durante uma execução, seguindo um fluxo lógico que pode ser alterado, se necessário.

Figuras como retângulos podem representar ações e losangos decisões a serem tomadas pela aplicação a partir de dados disponíveis, assim como linhas podem indicar o fluxo de execução entre os demais símbolos, e círculos podem unir linhas que se encontram para que seus fluxos continuem por um mesmo caminho. Observe o exemplo da imagem 2

![Fluxograma partindo de início e solicitando a inserção de um valor. Depois, é verificado se o valor é maior ou igual a zero. Caso seja, é exibida uma mensagem "VALOR POSITIVO". Caso contrário, é exibida a mensagem "VALOR NEGATIVO".](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a01-fig02.svg)

Imagem 2: Exemplo de fluxograma para analisar valor informado por usuário | Fonte: O autor.

Em relação ao que é mostrado acima, a solução lógica apresentada se refere ao mesmo problema desenvolvido na imagem 1, mas de uma forma diferente e mais intuitiva, baseada em formas que são padronizadas em significado, mas variando em sua aplicação e texto inserido nas mesmas para complementação do sentido de cada forma no diagrama.

Uma terceira forma de indicar uma solução computacional ainda não executável a princípio é por meio de algoritmos escritos usando pseudocódigos em uma linguagem conhecida como portugol em nosso país, e que podem ser escritos à mão de forma simplificada, usando pouca quantidade de texto em cada figura, mas possuindo alto poder de elaboração de soluções lógicas para problemas. Observe o exemplo na imagem 3.

INÍCIO

DECLARE

INTEIRO: VALOR;

LEIA (VALOR);

SE (VALOR > = 0)

ENTÃO

ESCREVA (“VALOR POSITIVO”);

SENÃO

ESCREVA (“VALOR NEGATIVO”);

FIMSE;

FIM.

Imagem 3: Exemplo de algoritmo | Fonte: O autor.

Neste algoritmo de exemplo na imagem 3, também se mostra uma alternativa para o mesmo problema proposto de identificação de um valor inserido por um usuário como positivo ou negativo, mas nesta solução existe um maior nível de detalhamento em função de uma maior proximidade com uma solução computacional.

Vários dos elementos utilizados no exemplo representam palavras que não podem ser utilizadas senão para o propósito ao qual se prestam, chamadas de palavras reservadas e que serão detalhadas ao longo dos estudos, e outros elementos que junto com estas palavras reservadas, constroem comandos em uma linguagem mais próxima das linguagens de programação, mas ainda mantendo uma leitura de fácil compreensão.

Um detalhe importante que deve ser colocado logo de início, é que qualquer uma das formas citadas de elaboração de soluções computacionais para problemas pode variar de uma fonte de pesquisa para outra. No exemplo da imagem 3, foi seguida a padronização de sintaxe do autor Forbellone, mas há outras formas de se escrever algoritmos variando, principalmente o uso de símbolos e algumas palavras reservadas, por exemplo.

*Machine Learning* (Aprendizado de Máquina) representa um dos diversos assuntos da área de TI e necessita de algoritmos muito bem elaborados para tratar de dados e como utilizá-los para que um *software* possa evoluir por meio de novas construções que possam ampliar uma base de informações existente.

Acesse o link:[Disponível aqui](https://www.sas.com/pt_br/insights/analytics/machine-learning.html)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Estrutura de um algoritmo

Os algoritmos representam conjuntos de instruções organizadas de forma a oferecer soluções lógicas para problemas computacionalmente possíveis. Um algoritmo deve ser claro e o mais otimizado possível, pois é apenas uma representação de uma solução, mas não a própria ainda, pois algoritmos precisam ser convertidos em alguma linguagem de programação desejada para se tornar um *software* e poder ser executado em um *hardware*.

Em geral, um algoritmo possui uma parte inicial em que são definidas estruturas de dados para armazenamento dos dados a serem processados na parte principal do algoritmo, e em geral, as estruturas de dados possuem tipos de dados aceitos definidos nessa parte inicial.

Após a definição das estruturas de dados, geralmente inicia-se a parte principal do algoritmo contendo todas as instruções necessárias para se solucionar problemas com base em entradas e saídas de dados e estruturas de controle, por exemplo. Observe o exemplo da imagem 4.

INÍCIO

DECLARE

INTEIRO: VALOR;

LEIA (VALOR);

SE (VALOR > = 0)

ENTÃO

ESCREVA (“VALOR POSITIVO”);

SENÃO

ESCREVA (“VALOR NEGATIVO”);

FIMSE;

FIM.

Imagem 4: Exemplo de algoritmo | Fonte: O autor.

No exemplo da imagem 4, temos o mesmo exemplo da imagem 3, mas com as duas seções básicas de um algoritmo separadas. Nas duas primeiras linhas é iniciado o algoritmo e definida a estrutura de dados a ser utilizada, e na segunda metade, o restante do algoritmo com a parte que desenvolve a solução em si, lembrando que cada algoritmo proposto para diferentes problemas geralmente possui diferentes instruções e estruturas de dados.

Pode haver outras partes em um algoritmo e estas serão aos poucos explicadas e exemplificadas para que se conheça mais a fundo a elaboração de algoritmos e a construção lógica de instruções, estruturas de controle, etc.

Uma prova da importância dos algoritmos está se concretizando em robôs autônomos e cada vez mais “inteligentes”, sendo capazes de tomar decisões mais complexas e de evoluir cada vez mais dentro de suas especificidades.

Existem *softwares* de auxílio funcionamento como atendentes virtuais em empresas para atendimentos mais simples e padronizados, assim como existem robôs que conseguem simular certos comportamentos humanos ou animais por meio de algoritmos capazes de realizar certo nível de “interpretação”.

A ideia é sempre observar as evoluções proporcionadas pela TI para si mesma ou para as demais áreas do conhecimento humano, e lembrar que para este desenvolvimento ocorrer, geralmente existem algoritmos utilizados para aplicar o que é proposto para gerar evoluções.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg)

## Palavras reservadas

As palavras reservadas servem como comandos para que cada ação a ser definida em um algoritmo seja padronizada através do uso de palavras definidas como padrão e cada uma delas tenha uma chamada sintaxe que define os elementos necessários e opcionais para a composição de instruções utilizando estas palavras reservadas como elemento principal de cada instrução.

Estas palavras são utilizadas também em todas as linguagens de programação, pois esta padronização, além de facilitar o aprendizado e uso na elaboração de algoritmos, é necessária para que compiladores e interpretadores possam compreender as ações e a lógica que foi definida pelas instruções em uma linguagem de programação qualquer.

Observe a tabela 1 que traz uma lista de palavras reservadas a serem utilizadas neste material e uma breve descrição de suas funcionalidades.

| **PALAVRA RESERVADA** | **DESCRIÇÃO** |
| --- | --- |
| ABRA | AÇÃO PARA ARQUIVO |
| ARQUIVO COMPOSTO DE | DECLARAÇÃO DE ARQUIVO |
| ATE | FINAL DE COMANDO DE REPETIÇÃO |
| ATÉ | COMPLEMENTO DE COMANDO DE REPETIÇÃO |
| ATRIBUTO | CARACTERÍSTICA DE UM OBJETO |
| CARACTERE | TIPO DE DADO |
| CASO | COMANDO CONDICIONAL |
| CLASSE | DESCRIÇÃO PARA GERAR ABSTRAÇÃO DE OBJETO |
| CONJUNTO | TIPO DE DADO |
| COPIE | AÇÃO PARA ARQUIVO |
| DE | COMPLEMENTO DE COMANDO DE REPETIÇÃO |
| DECLARE | SEÇÃO DE DECLARAÇÃO DE VARIÁVEIS |
| ELIMINE | AÇÃO PARA ARQUIVO |
| ENQUANTO | COMANDO DE REPETIÇÃO |
| ENTÃO | COMPLEMENTO DE COMANDO CONDICIONAL |
| ESCREVA | SAÍDA DE DADOS |
| FAÇA | COMPLEMENTO DE COMANDO DE REPETIÇÃO |
| FECHE | AÇÃO PARA ARQUIVO |
| FIM | FINAL DE BLOCO DE INSTRUÇÕES |
| FIM\_REGISTRO | FINAL DE DECLARAÇÃO DE REGISTRO |
| FIMCASO | FINAL DE COMANDO CONDICIONAL |
| FIMENQUANTO | FINAL DE COMANDO DE REPETIÇÃO |
| FIMPARA | FINAL DE COMANDO DE REPETIÇÃO |
| FIMSE | FINAL DE COMANDO CONDICIONAL |
| FUNÇÃO | INÍCIO DE SUB-ROTINA |
| GUARDE | AÇÃO PARA ARQUIVO |
| INÍCIO | INÍCIO DE BLOCO DE INSTRUÇÕES |
| INTEIRO | TIPO DE DADO |
| LEIA | ENTRADA DE DADOS |
| MÉTODO | AÇÃO QUE PODE SER EFETUADA POR UM OBJETO |
| PARA | COMANDO DE REPETIÇÃO |
| PASSO | COMPLEMENTO DE COMANDO DE REPETIÇÃO |
| PROCEDIMENTO | INÍCIO DE SUB-ROTINA |
| REAL | TIPO DE DADO |
| REGISTRO | INÍCIO DE DECLARAÇÃO DE REGISTRO |
| REPITA | COMANDO DE REPETIÇÃO |
| SE | COMANDO CONDICIONAL |
| SEJA | COMPLEMENTO DE COMANDO CONDICIONAL |
| SENÃO | COMANDO CONDICIONAL |
| TIPO | COMPLEMENTO DE COMANDO DE REGISTRO |

Tabela 1: Exemplo de algoritmo | Fonte: O autor.

Nesta tabela 1, foram incluídas as palavras reservadas para os estudos neste material, e as palavras utilizadas seguem como base os autores Manzano e Forbellone que em seus livros, utilizaram conjuntos semelhantes de palavras reservadas, mas parte delas é encontrada apenas no material de Forbellone relativo à parte sobre arquivos, mas o restante das palavras foi baseado no que foi descrito por Manzano.

Conhecer as palavras reservadas de uma linguagem não é uma obrigação, mas se torna cada vez mais automática a escolha de cada palavra a utilizar em cada situação, e quais os elementos adicionais utilizáveis com cada palavra à medida que se desenvolvem os estudos na área e se realiza a prática de desenvolvimento de algoritmos para resolver diferentes tipos e complexidades de problemas.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Formas de representação de soluções de problemas
- Estrutura de um algoritmo
- Palavras reservadas

Para complementar seus estudos, assista à videoaula a seguir: