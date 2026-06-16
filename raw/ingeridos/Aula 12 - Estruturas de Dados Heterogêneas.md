---
title: "Aula 12 - Estruturas de Dados Heterogêneas"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-12.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 12 - Estruturas de Dados Heterogêneas

Sumário[1\. Estruturas de dados heterogêneas](#topico-01)[

2\. Registros

](#topico-02)

## Estruturas de dados heterogêneas

As estruturas de dados vêm sendo incrementadas nas duas últimas aulas e a quantidade de dados que podem ser inseridos nestas estruturas é grande, mas com a limitação de que todos os dados sejam de um mesmo tipo.

Existe um tipo adicional de estrutura de dados a ser estudado neste material que permite que uma mesma estrutura possa conter dados de diferentes tipos sob um mesmo nome, mas é importante observar que a forma como se referenciam os dados em estruturas deste tipo é diferente das demais estudadas até então.

É comum que este tipo de estrutura seja chamado de registro ou de estrutura em algumas linguagens de programação e podem gerar alguma confusão em função de outras linguagens ou aplicações da área de tecnologia da informação utilizarem estes dois termos com finalidades distintas.

De qualquer maneira, para convencionar os estudos neste material será utilizado o termo registro em função do uso da palavra estrutura como um termo genérico para estruturas de dados.

Em certos momentos dos estudos, os conceitos de algoritmos se misturam com conceitos de outras áreas da TI, e um destes momentos ocorre nesta aula onde a base para a teoria de bancos de dados se mistura com a de estruturas de dados homogêneas e heterogêneas.

Acesse o link:[Disponível aqui](https://www.devmedia.com.br/conceitos-fundamentais-de-banco-de-dados/1649)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

## Registros

TIPO CADASTRO = REGISTRO

INTEIRO: CODIGO, IDADE;

CARACTERE: NOME, ENDEREÇO, CIDADE, ESTADO

FIMREGISTRO;

CADASTRO: DADOS;

Imagem 38: Exemplo de estrutura de decisão em estrutura de repetição.| Fonte: O autor.

No exemplo trazido na imagem 38 é declarada uma estrutura de dados do tipo registro com o nome de “CADASTRO” após o uso da palavra reservada “TIPO” e antes da sequência “= REGISTRO” que são elementos padrões da sintaxe e que sempre serão utilizados desta forma na escrita de algoritmos.

Em seguida, no exemplo são declarados campos para o registro que seguem os padrões de sintaxe das variáveis comuns, indicando primeiramente o tipo de dado aceito, seguido do símbolo “:”. Depois, um ou mais nomes de campos podem ser inseridos se forem todos do mesmo tipo, separados por vírgulas e finalizados pelo símbolo padrão “;” como em praticamente todas as demais instruções.

Após a declaração de todos os campos desejados com a indicação dos respectivos tipos, ao final, utiliza-se a palavra reservada “FIMREGISTRO” para encerrar a declaração da estrutura de dados do tipo registro, seguido do símbolo “;”.

Assim, com a declaração do registro, o que se tem na verdade, é um novo tipo de dados definido pelo desenvolvedor, e que pode ser utilizado na declaração de variáveis simples.

Esse recurso permite que uma variável declarada com um tipo de registro de dados possa ser então preenchida com dados e manipulada normalmente por um algoritmo no qual esteja declarada. A imagem 39 traz a forma como se pode utilizar a variável declarada no exemplo da imagem 38.

LEIA (DADOS.CODIGO);

LEIA (DADOS.NOME);

LEIA (DADOS.IDADE);

LEIA (DADOS.ENDERECO);

LEIA (DADOS.CIDADE);

LEIA (DADOS.ESTADO);

ESCREVA (“REGISTRO NÚMERO: “, DADOS.CODIGO);

ESCREVA (“NOME: “, DADOS.NOME);

ESCREVA (“IDADE: “, DADOS.IDADE);

ESCREVA (“ENDEREÇO: “, DADOS.ENDEREÇO);

ESCREVA (“LOCAL: “, DADOS.NOME, “–“, DADOS.ESTADO);

Imagem 39: Exemplo de uso de variável declarada como registro.| Fonte: O autor.

Neste exemplo da imagem 39, complementar ao da imagem 38, temos o uso da estrutura de dados do tipo registro definida e posteriormente utilizada na declaração de uma variável “DADOS”.

Neste trecho de algoritmo são utilizados comandos de entrada e saída de dados para que seja possível a entrada de dados para os campos do registro com o comando LEIA, e depois sejam reexibidos de forma formatada com informações complementares ao usuário com o comando ESCREVA.

Compreender a forma de uso para estruturas heterogêneas é bastante importante, visto que são estruturas desiguais, e assim, aceitam dados de tipos diferentes, podendo aumentar rapidamente a complexidade da elaboração de algoritmos utilizando estes tipos de estruturas de dados, ainda mais se utilizadas em conjunto com vetores para a criação de listas de registros a serem manipulados em tempos de execução.

Fonte:[Disponível aqui](https://educacao.uol.com.br/disciplinas/portugues/giria-e-jargao-a-lingua-mudaconforme-situacao.htm)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Estruturas de dados heterogêneas
- Registros

Para complementar seus estudos, assista à videoaula a seguir: