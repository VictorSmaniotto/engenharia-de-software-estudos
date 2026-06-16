---
title: "Aula 06 - Entrada e Saída de Dados"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-06.html"
author:
published:
created: 2026-05-28
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 06 - Entrada e Saída de Dados

Sumário

## Entrada de Dados

Após os estudos sobre dados simples, é preciso compreender como é possível obter dados para manipulação em um algoritmo. Este é um dos fundamentos da elaboração de algoritmos, pois é o recurso que permite a interatividade fundamental entre usuário e algoritmo.

A princípio, o processo de entrada de dados mais comum é a digitação de dados pelo usuário que serve como periférico padrão para interação com algoritmos, mas há outras formas como leitura de dados gravados em arquivos, dados obtidos em redes de computadores, ou até na rede mundial Internet.

Para os estudos deste material, será inicialmente tratada apenas a entrada de dados via teclado, pois é uma forma comum de realização deste processo e a mais simples de entendimento em uma etapa de iniciação nos estudos em relação ao desenvolvimento de *software*.

A palavra reservada “LEIA” é utilizada como comando para a elaboração de instruções de entrada de dados e sua sintaxe para construção de instruções é bastante simples. Observe o exemplo da imagem 13.

LEIA (X);

LEIA (IDADE);

LEIA (PESO, ALTURA);

Imagem 13: Exemplos de entrada de dados. | Fonte: O autor.

Nestes exemplos da imagem 13, a mesma palavra reservada padrão “LEIA” é utilizada e isto mostra que é simples o seu uso, por ser um comando único para a função deste estudo.

No primeiro exemplo, o comando solicita a digitação de um dado para uma variável “X” que espera a inserção de um dado quando executado o algoritmo, da mesma forma que o segundo exemplo, mas este, utiliza como estrutura de dados para armazenamento temporário, uma variável “IDADE” que pelo nome, possui um significado mais claro de sua finalidade em relação ao nome dado à variável do primeiro exemplo.

Este detalhe de escolha de nomes é importante, pois à medida que se desenvolvem códigos cada vez maiores, uma maior quantidade de variáveis e outras estruturas de dados podem ser declarados, e nomes muito genéricos utilizados como identificadores para estas estruturas de dados prejudica a interpretação de algoritmos.

Como dica é bom sempre pensar em nomes intuitivos e bem claros em seu significado, mesmo que formados por palavras compostas, lembrando que não é permitido o uso de espaços em nomes e por isto, pode-se criar nomes com as partes compostas todas unidas ou usando o símbolo “\_” permitido na elaboração de nomes em algoritmos e em linguagens de programação normalmente.

Ilustrativa | Fonte: @nd3000

[Disponível aqui](https://elements.envato.com/pt-br/programador-trabalhando-em-uma-empresa-de-4KR8QF3)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a05-img1.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg)

Nomes como “PESOMAXIMO” ou “PESO\_MINIMO” são aceitos sem problemas e possuem um significado bastante intuitivo para interpretação do tipo de dado que poderá estar contido nestas estruturas de dados.

No terceiro exemplo da imagem 18, é importante observar que é permitido que uma instrução de entrada de dados possa incluir mais de uma variável por vez, separando seus nomes com o símbolo “,” quando colocadas dentro dos parênteses do comando “LEIA”.

Assim, neste terceiro exemplo, foram solicitadas as digitações de dados para as variáveis “PESO” e “ALTURA” em uma mesma instrução, e o usuário poderá digitar os dois dados em sequência, sendo necessário que a cada dado inserido, seja pressionada a tecla “ENTER” para finalizar a inserção e poder então passar à digitação de outro dado para outra variável solicitada numa instrução, ou para que a execução normal do algoritmo prossiga.

A entrada de dados é fundamental para um algoritmo, pois é a interação com usuário que ocorre por este mecanismo. Um recurso bastante útil e que deve se tornar uma prática comum é o uso de validações para redução de entradas de dados incorretas.

Estruturas de dados são tipadas para que os tipos de dados adequados sejam inseridos, mas há também casos em que existem exceções que necessitam ser tratadas, como no caso da realização de uma operação de divisão, que o segundo valor a ser utilizado como divisor não pode ser zero, pois isto gera um erro em função de não ser possível esta operação.

Pode-se então, incluir um mecanismo no algoritmo para verificar um valor recebido por uma variável, e caso seja zero, um novo valor diferente deve ser solicitado ou atribuído a uma variável.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

## Saída de Dados

O processo que complementa a entrada de dados e o processamento destes é a saída de dados que também pode ser realizada de diferentes maneiras, como a exibição de dados em tela que é a opção padrão para esta atividade, a gravação em disco que também é bastante comum, o envio por meio de redes de computadores, ou como na entrada de dados, até como envio de dados pela *web*.

Para esta aula a saída de dados padrão em tela será a única explorada, pois também sendo a opção padrão, é a mais adequada para este ponto dos estudos, mas a implementação de instruções com comandos de saída é um pouco mais complexa que na entrada de dados.

Neste tipo de instrução de saída, utiliza-se a palavra reservada “ESCREVA” que também necessita de parâmetros inseridos entre parênteses para a estruturação de instruções de saída, mas é possível mesclar diferentes tipos de parâmetros neste tipo de comando. Observe os exemplos da imagem 14.

ESCREVA (“Texto Exemplo”);

ESCREVA (IDADE);

ESCREVA (PESO, “ – “, ALTURA);

ESCREVA (“Nome: “, NOME);

ESCREVA (“O valor da média entre “, VALOR1, “ e ”, VALOR2, “ é: “, MEDIA);

Imagem 14: Exemplos de saída de dados. | Fonte: O autor.

Nos exemplos trazidos na figura 14, o primeiro exemplo traz apenas uma mensagem a ser exibida ao usuário, indicada entre aspas que fazem parte da sintaxe do comando “ESCREVA” e devem sempre ser utilizadas em caso de exibição de mensagens.

Um detalhe importante é que as mensagens entre aspas não representam palavras reservadas da linguagem ou nomes de estruturas de dados, e por isso, o texto a ser inserido pode conter qualquer conjunto de caracteres formando ou não palavras, em letras maiúsculas ou minúsculas, símbolos diversos do teclado, e números, por exemplo.

No segundo exemplo, apenas o nome de uma variável “IDADE” é utilizado, e esta instrução apenas exibirá o dado contido na variável, que pelo seu nome, imagina--se que seja um número inteiro, pelas características deste tipo de informação.

Assim, percebe-se que não é obrigatório o uso de aspas em todas as instruções de saída de dados, sendo então livre a composição de instruções de saída utilizando texto ou variáveis em quantidades variadas.

O terceiro exemplo já mescla estes elementos como parâmetros do comando de saída, e é importante observar que cada elemento a ser exibido, por serem distintos, devem ser separados pelo símbolo “,” que no momento da exibição concatena todos os parâmetros contidos no comando em sequência para serem exibidos ao usuário, e por isto que neste exemplo o texto utilizado “–” contém espaço em branco antes e depois do traço, para evitar que os dados das variáveis apareçam emendados ao símbolo de traço.

O quarto exemplo é bem típico em algoritmos e mostra ao usuário o dado contido na variável nome, mas antes informa por meio do texto entre aspas que tipo de informação está sendo passada, deixando assim, a aparência da mensagem semelhante à de um formulário de dados comum.

O quinto exemplo é o mais complexo e contém vários parâmetros que unidos, exibem uma informação completa ao usuário. O conteúdo “(“O valor da média entre “, VALOR1, “ e ”, VALOR2, “ é: “, MEDIA)” parece bastante complexo, mas na verdade facilita a compreensão se forem separados os elementos a partir das vírgulas, e assim, temos os parâmetros indicados na imagem 15.

“O valor da média entre“ - Mensagem simples a ser exibida

VALOR1 - Valor da variável VALOR1 a ser exibido

“ e ” - Mensagem simples a ser exibida

VALOR2 - Valor da variável VALOR2 a ser exibido

“ é: “ - Mensagem simples a ser exibida

MEDIA - Valor da variável MEDIA a ser exibido

Imagem 15: Separação dos parâmetros do exemplo da imagem 19. | Fonte: O autor.

A concatenação ou união entre estes elementos exibe na tela algo como “O valor da média entre 10 e 2 é: 5”, por exemplo, imaginando que foram inseridos os valores 10 e 2 para as variáveis “VALOR1” e “VALOR2”, respectivamente, e o valor para a variável “MEDIA” foi obtido a partir do cálculo da média entre os dois valores.

Após conhecer a ideia de entrada e saída de dados, é interessante complementar os estudos conhecendo a parte de entrada e saída de dados de *hardware*, pois os algoritmos podem utilizar estes recursos para realizar estes dois processos.

Acesse o link:[Disponível aqui](https://www.diferenca.com/dispositivos-de-entrada-e-saida/)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Analisando um Primeiro Algoritmo Completo

Após conhecer parte dos conceitos fundamentais do desenvolvimento de algoritmos, é possível avaliar um exemplo completo de algoritmo para compreender a aplicação do que foi estudado até então e compreender melhor o uso de cada conceito visto até então.

Partindo de um problema tema para o algoritmo, pode-se simular o desenvolvimento de uma possível solução computacional lembrando que não existe apenas uma solução possível para cada problema, mas sim, variações possíveis que contemplam funcionalidades semelhantes ou iguais, podendo ser implementadas de diferentes formas e com variações na lógica inclusive.

Observe a imagem 16 para um exemplo completo de algoritmo que se propõe a receber três valores, e retornar a média entre estes valores, lembrando que para este cálculo é preciso somar os três valores e dividir esta soma por três para obter o resultado esperado.

INÍCIO

DECLARE

REAL VALOR1, VALOR2, VALOR3, MEDIA;

ESCREVA (“DIGITE UM PRIMEIRO VALOR: “);

LEIA (VALOR1);

ESCREVA (“DIGITE UM SEGUNDO VALOR: “);

LEIA (VALOR2);

ESCREVA (“DIGITE UM TERCEIRO VALOR: “);

LEIA (VALOR3);

MEDIA <- (VALOR1 + VALOR2 + VALOR3) / 3;

ESCREVA (“A MÉDIA ENTRE OS TRÊS VALORES É “, MEDIA);

FIM.

Imagem 16: Separação dos parâmetros do exemplo da imagem 20. | Fonte: O autor.

Neste algoritmo da imagem 16, é possível observar todos os detalhes de estrutura de um algoritmo comum e os principais conceitos estudados até então, desde a primeira aula.

Como de costume na elaboração de algoritmos, inicia-se um algoritmo com a palavra reservada “INÍCIO” e na sequência, a palavra reservada “DECLARE” inicia a etapa de declaração de variáveis para uso no algoritmo.

São declaradas quatro variáveis “VALOR1”, “VALOR2” e “VALOR3” para receber os dados a serem informados pelos usuários para o cálculo como solicitado como requisito para o algoritmo. Por fim, é declarada uma quarta variável “MEDIA” para receber, posteriormente, o resultado do cálculo a ser realizado com os dados contidos nas três outras variáveis declaradas no algoritmo.

Em seguida, uma sequência de comandos “ESCREVA” e “LEIA” realizam a função de informar ao usuário que ele deve digitar um primeiro valor, para em seguida solicitar a digitação do valor em si através de um “ *prompt* ” para inserção de dados pelo teclado.

Este processo é repetido por três vezes a fim de que os dados para as três variáveis bases para o cálculo da média sejam preenchidos com valores que podem ser inteiros ou decimais em função do tipo “REAL” definido na declaração das variáveis.

Ilustrativa | Fonte: @nd3000

[Disponível aqui](https://elements.envato.com/pt-br/engenheiros-de-software-que-trabalham-em-projeto-TWXZ4UK)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a05-img2.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg)

Depois da obtenção dos dados, uma atribuição é realizada para a variável “MEDIA” que recebe o resultado da soma e posterior divisão dos valores contidos nas três variáveis para obtenção da média solicitada.

Por fim, após inserção do resultado do cálculo na variável “MEDIA”, o valor da mesma é utilizado no comando de saída de dados “ESCREVA” para exibir uma mensagem informando o resultado do cálculo da média com o valor obtido.

Aplicações em geral possuem entradas e saídas de dados para interação com usuários. Algumas aplicações podem ser totalmente automatizadas e não dependerem de nenhum tipo de interação humana, mas em geral, a possibilidade de interação existe e é importante em uma grande quantidade de algoritmos.

Existem sistemas complexos que necessitam de entradas de dados como os chamados ERPs (*Enterprise Resource Planning* ou Sistema de Gestão Empresarial) que recebem e manipulam grandes quantidades de dados em negócios diversos, jogos, *softwares* aplicativos em geral, etc.

Implementar algoritmos com mensagens de auxílio ao correto preenchimento de entradas de dados, por exemplo, é um bom exemplo de uso de saídas e entradas de dados em conjunto, muito comuns em aplicações de todo tipo.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Entrada de Dados
- Saída de Dados
- Analisando um Primeiro Algoritmo Completo

Para complementar seus estudos, assista à videoaula a seguir: