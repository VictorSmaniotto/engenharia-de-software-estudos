---
title: "Aula 07 - Estruturas de Decisão"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-07.html"
author:
published:
created: 2026-05-28
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 07 - Estruturas de Decisão

Sumário

## Estruturas de Controle

Após os estudos de tipos, variáveis e os recursos de interatividade para entrada e saída de dados, já é possível avançar nos estudos e conhecer novos recursos de programação capazes de influenciar o chamado fluxo de execução da aplicação.

Esse fluxo representa a ordem de execução das instruções e por meio dos recursos estudados até então, os algoritmos poderiam ser executados apenas de forma sequencial, sem opções de escolhas na forma como as instruções são executadas, ou até se devem ser executadas em determinadas situações controladas pelo próprio algoritmo.

As chamadas estruturas de controle representam meios de definir critérios para que determinadas instruções ou blocos de instruções sejam executadas ou não dependendo de condições pré-determinadas no código, e que afetam a execução dos algoritmos.

## Estrutura de Decisão Condicional Simples

Uma estrutura de decisão condicional simples representa um recurso de controle de fluxo de execução que se baseia em uma condição controlada pelo algoritmo em tempo de execução que define se uma ou mais instruções devem ser executadas ou não.

A ideia do uso de uma condição para a execução de instruções remete ao conteúdo visto na aula 4 em que alguns tipos de operadores não realizavam cálculos, mas serviam para avaliar expressões com o objetivo de retornar valores verdadeiros ou falsos, perfeitos para o tipo de condição utilizável neste tipo de estrutura de controle.

Estas expressões condicionais devem ser muito bem elaboradas, pois desvios incorretos causados por erros lógicos associados a condições equivocadas em sua elaboração comprometem funcionalidades de algoritmos e podem gerar problemas como instruções que nunca são executadas ou executadas em momentos inoportunos.

A palavra reservada mais conhecida para este tipo de instrução é “SE” e possui uma sintaxe bem simples para sua estruturação, sendo que os maiores problemas em seu uso são ocasionados pelas condições elaboradas para as instruções. Observe o exemplo da imagem 17 para compreender como se pode estruturar um comando deste tipo.

SE (VALOR > = 0) ENTÃO

ESCREVA(“NÚMERO POSITIVO“);

FIMSE;

Imagem 17: Exemplo de estrutura condicional simples. | Fonte: O autor.

Neste exemplo da imagem 17, um comando condicional simples é implementado com o objetivo de avaliar o valor contido na variável “VALOR”, e caso contenha um valor numérico maior ou igual a zero, é exibida uma mensagem informando que o número digitado é positivo.

É importante neste exemplo observar a sintaxe do comando, em que após o uso da palavra reservada “SE”, a condição é inserida na instrução, que neste caso, verifica se o valor contido na variável “VALOR” é maior ou igual a zero para que a mensagem adequada seja exibida.

A sintaxe básica de um comando utilizando a palavra reservada “SE” inicia pela palavra, seguida por uma expressão condicional normalmente entre parênteses, e por fim, outra palavra reservada “ENTÃO” para, na sequência, ser colocada uma instrução ou bloco de instruções a serem executadas apenas quando a expressão condicional resultar verdadeiro.

Assim, no exemplo específico da imagem 17, a mensagem “NÚMERO POSITIVO” seria exibida quando o dado contido na variável “VALOR” desse exemplo for qualquer número maior ou igual a zero.

Na linha seguinte, é inserida uma instrução para exibir ao usuário uma mensagem, lembrando que esta será exibida apenas em caso de a expressão resultar verdadeiro, e o dado contido na variável “VALOR” ser realmente positivo. Para encerrar a instrução de controle de decisão simples, utiliza-se a palavra reservada “FIMSE”.

## Estrutura de Decisão Composta

Partindo do que foi estudado na estrutura de decisão simples, foi visto a importância de se poderem criar opções na execução de algoritmos além da sequencial execução de instruções sem desvios na ordem em que são executadas.

A estrutura de decisão composta é um tipo mais completo de estrutura de decisão, pois permite que se tenha duas opções de instruções a serem executadas a partir do resultado de expressões condicionais, e para isto uma nova palavra reservada “SENÃO” é adicionada para implementação deste tipo de instrução.

Observe o exemplo da imagem 18 para conhecer a sintaxe deste tipo de instrução e compreender o que pode ser agregado a uma estrutura de controle para decisão a partir desta variação da construção deste tipo de instrução.

SE (VALOR > = 0) ENTÃO

ESCREVA (“NÚMERO POSITIVO“);

SENÃO

ESCREVA (NÚMERO NEGATIVO”);

FIMSE;

Imagem 18: Exemplo de estrutura condicional simples. | O autor.

Observando o exemplo da imagem 18, é possível perceber que a mesma instrução de controle de fluxo possui agora duas instruções de exibição de mensagem ao usuário.

A primeira será exibida apenas se o dado contido na variável “VALOR” for positivo, ao passo que em caso de a expressão condicional resultar falso e o dado contido for negativo, a outra mensagem é automaticamente executada.

Com isso é possível que um algoritmo possa controlar a execução de instruções de forma adequada para dados que vão sendo avaliados em tempo de execução, por exemplo, permitindo que sejam criados algoritmos mais dinâmicos.

Estruturas de decisão trazem um adicional importante para o desenvolvimento de algoritmos e devem ser cuidadosamente utilizados, pois envolvem desvios na execução de algoritmos e equívocos na estruturação destas instruções pode acarretar processamento incorreto de dados ou até de perda de funcionalidade.

Sempre é importante avaliar as expressões condicionais utilizadas, testar seus possíveis resultados e validar se a condição funcionará como desejado, reduzindo as chances de ocorrências de erros em tempo de execução.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

## Estrutura de Decisão Aninhada

O uso de estruturas de decisão permite que se possa controlar o fluxo de execução de um algoritmo, mas para todas as situações ter duas alternativas é suficiente?

Há casos em que pode ser necessário que se tenha mais de duas alternativas de escolha de desvio de fluxo, como, por exemplo, na escolha entre decisões a serem executadas a partir da escolha entre cores.

Uma das situações mais comuns que podem gerar a necessidade de maior possibilidade de escolhas é na implementação de menus de opções em que cada escolha pode desviar o fluxo de execução de um algoritmo para diferentes conjuntos de instruções. Observe o exemplo da imagem 19 para melhor compreensão deste tipo de situação.

SE (OPCAO = 1) ENTÃO

ESCREVA (“A OPÇÃO ESCOLHIDA FOI A PRIMEIRA“);

SENÃO SE (OPCAO = 2) ENTÃO

ESCREVA (“A OPÇÃO ESCOLHIDA FOI A SEGUNDA”);

SENÃO SE (OPCAO = 3) ENTÃO

ESCREVA (“A OPÇÃO ESCOLHIDA FOI A TERCEIRA”);

SENÃO SE (OPCAO = 4) ENTÃO

ESCREVA (“A OPÇÃO ESCOLHIDA FOI A QUARTA”);

SENÃO

ESCREVA (“OPÇÃO DESCONHECIDA”);

FIMSE;

FIMSE;

FIMSE;

Imagem 19: Exemplo de estrutura condicional composta. | Fonte: O autor.

Tendo como base o exemplo da imagem 19, observa-se que existem múltiplas opções sendo tratadas em uma composição de instruções baseadas no comando “SE” que são organizadas de forma a fazerem parte de uma estrutura única em que no caso de uma das condições ser verdadeira, não há o risco de as instruções contidas nas demais serem executadas.

A estrutura deve ser organizada de forma que cada nova estrutura de decisão seja implementada como a alternativa falsa da estrutura anterior, fazendo assim com que cada nova estrutura esteja agregada à estrutura anterior, e assim, para melhor compreensão do algoritmo, aconselha-se a endentação (espaçamento) mais à direita para cada nova estrutura que seja aninhada.

No caso específico desse exemplo da imagem 19, a ordem de execução das estruturas aninhadas se baseia na ideia de que primeiro é avaliado se o valor contido na variável “OPCAO” é igual a 1. Caso seja, executará a instrução referente e não executará o conteúdo de “SENÃO” que contém todo o restante das estruturas aninhadas, e assim, encerra-se toda esta estrutura aninhada.

Caso a primeira condição resulte falsa, a estrutura parte para a avaliação do “SENÃO” que traz toda a estrutura aninhada que realiza nova avaliação do valor contido na variável “OPCAO”, e caso seu valor seja 2, resulta verdadeiro e a instrução contida na estrutura é executada.

Ilustrativa | Fonte: DragonImages

[Disponível aqui](https://elements.envato.com/pt-br/codigo-de-escrita-do-programador-trabalhador-2WB2H6D)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a07-img2.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg)

Pode ocorrer desta segunda condição resultar falsa também, e assim, o algoritmo passa a avaliar a próxima estrutura contida no “SENÃO” desta segunda estrutura que contém outro aninhamento de estruturas condicionais.

Nesta terceira avaliação, caso a condição resulte verdadeira pela variável conter o valor 3, a instrução que pertencente a esta estrutura é executada, mas caso resulte falsa, novamente segue-se para o conteúdo contido agora em “SENÃO” desta estrutura que agora avalia se o valor contido na variável “OPÇÃO” é igual a 4.

Caso seja verdadeira a expressão, executa a instrução contida, mas caso seja falsa, executa agora o comando “SENÃO” sem mais nenhuma estrutura aninhada e nem condição a ser avaliada, e assim, qualquer valor diferente dos demais avaliados anteriormente entre 1 a 4 resultará na execução da instrução contida nesta última opção.

Outra forma de se aninhar estruturas de decisão é por meio da complementação entre condições, em que uma deve ser avaliada apenas se uma outra anterior tiver um resultado esperado para esta segunda estrutura. Observe o exemplo da imagem 20.

SE (DOCUMENTO = VERDADEIRO) ENTÃO

SE (IDADE >= 18) ENTÃO

ESCREVA (“ENTRADA PERMITIDA”)

SENÃO

ESCREVA (“MENOR DE IDADE”);

SENÃO

ESCREVA (“SEM DOCUMENTO”);

FIMSE;

Imagem 20: Exemplo de estrutura condicional aninhada. | Fonte: O autor.

Neste exemplo da imagem 20 ocorre uma situação também bastante comum no desenvolvimento de algoritmos em que a avaliação de uma pessoa estar ou não devidamente documentada para que possa então ser verificado o documento em relação à idade da pessoa.

Para isto, são avaliados os valores contidos primeiramente na variável “DOCUMENTO”, e caso seja “VERDADEIRO”, a segunda estrutura condicional é iniciada e é então verificado se o valor contido na variável “IDADE” é maior ou igual a 18. Se tanto a primeira, quanto a segunda condição forem verdadeiras, é exibida a mensagem de ‘entrada permitida’, mas se a segunda condição resultar falsa, é exibida a mensagem de a pessoa ser menor de idade. Por fim, se a primeira condição resultar falsa, a segunda nem é avaliada e já é exibida uma mensagem informando a falta de documentação.

Complementando o que já foi citado sobre operadores e expressões, as estruturas de controle de fluxo baseados em estruturas de decisão simples, compostas ou de seleção múltipla, todas estas estruturas necessitam de expressões para que se possam definir quando e se trechos de algoritmos devem ser executados.

As estruturas de decisão são essenciais na elaboração de algoritmos que realizam verificações relacionadas a dados como datas, idades, verificações de palavras, validações de dados, etc.

É importante compreender como se elaboram instruções condicionais para que se possam automatizar cada vez mais os processos, e assim, criar algoritmos cada vez mais complexos, completos e eficientes.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg)

## Estrutura de Seleção Múltipla

Por último, existe um tipo mais específico de estrutura de decisão para quando uma variável pode definir ao menos dois ou mais valores distintos de uma variável que podem ser utilizados como critérios para a escolha entre instruções a serem ou não executadas. Um exemplo de uso deste tipo de estrutura é trazido na imagem 21:

ESCOLHA OPCAO

CASO 1: ESCREVA (“A OPÇÃO ESCOLHIDA FOI A PRIMEIRA“);

CASO 2: ESCREVA (“A OPÇÃO ESCOLHIDA FOI A SEGUNDA”);

CASO 3: ESCREVA (“A OPÇÃO ESCOLHIDA FOI A TERCEIRA”);

CASO 4: ESCREVA (“A OPÇÃO ESCOLHIDA FOI A QUARTA”);

CASO CONTRÁRIO: ESCREVA (“OPÇÃO DESCONHECIDA”);

FIMESCOLHA;

Imagem 21: Exemplo de estrutura de seleção múltipla. | Fonte: O autor.

Por meio do exemplo trazido na imagem 21, a alternativa de implementação do trecho de algoritmo mostrado na imagem 19 parece muito mais simples em sua lógica, interpretação e escrita, mas é preciso observar que este tipo de estrutura serve apenas para casos em que um único valor deve ser avaliado em relação a uma variável, e não é possível a composição de expressões lógicas ou relacionais como utilizadas no comando “SE”.

A escolha entre utilizar um tipo de estrutura de decisão SE...SENÃO ou ESCOLHA...CASO é simples, pois a segunda opção é bastante restrita a algumas situações, mas para um estudo complementar, segue link para material de apoio.

Acesse o link:[Disponível aqui](http://uab.ifsul.edu.br/tsiad/conteudo/modulo1/lop/lop_ud/lop_03.html)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Estruturas de Controle
- Estrutura de Decisão Condicional Simples
- Estrutura de Decisão Composta
- Estrutura de Decisão Aninhada
- Estrutura de Seleção Múltipla

Para complementar seus estudos, assista à videoaula a seguir: