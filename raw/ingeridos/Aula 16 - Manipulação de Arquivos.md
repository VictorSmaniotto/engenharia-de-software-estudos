---
title: "Aula 16 - Manipulação de Arquivos"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-16.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 16 - Manipulação de Arquivos

Sumário[1\. Manipulação de Arquivos de Texto](#topico-01)## Manipulação de Arquivos de Texto

Os dados manipulados durante a execução de algoritmos são normalmente perdidos ao final do processo, pois são todos alocados em estruturas de dados em memória temporária, a menos que sejam enviados pela *web* ou gravados em unidades físicas, por exemplo, não se podem recuperar dados processados em uma nova execução do mesmo algoritmo ou por outros algoritmos.

Para que dados processados possam estar disponíveis para uso após o encerramento da execução de um algoritmo, é preciso que sejam criados meios para que estes sejam armazenados de forma permanente e não apenas de forma temporária.

O uso de arquivos de texto ou binários é uma forma eficiente de se ter dados disponíveis sempre, permitindo a adição, consulta, edição ou exclusão dos mesmos a qualquer momento pela execução de algoritmos implementados com recursos de uso de arquivos.

Como os arquivos do tipo binário representam recursos muito mais complexos em sua manipulação, serão deixados de lado e o foco da aula será o uso de arquivos de texto para armazenamento de dados com base em caracteres textuais de forma geral.

Um arquivo é uma estrutura controlada pelo sistema operacional, e por isto, o desenvolvimento de algoritmos precisa se atentar aos detalhes dos sistemas operacionais para a implementação de certas funcionalidades, como na forma como se nomeiam arquivos nos diferentes sistemas operacionais e como são manipulados.

Arquivos de texto contêm conteúdo não necessariamente estruturado, e por isto, caso seja necessária a organização do conteúdo a ser mantido em um arquivo, é importante incluir em toda a documentação dos algoritmos, a forma como devem ser organizados os dados em arquivos, caracteres especiais que serão utilizados como separadores ou palavras-chave que serão inseridas junto ao conteúdo para melhor organização, se necessário.

Como esse tipo de arquivo possui tamanho bastante reduzido, geralmente é possível que uma grande quantidade de dados possa ser armazenada, e assim, sua utilidade e finalidades as quais possam ser aplicadas aumentam, fazendo deste recurso um componente importante a ser considerado na elaboração de algoritmos para aplicações que necessitem de dados gravados.

Assim, é possível imaginar arquivos de texto em que cada linha do mesmo representa um conjunto de dados referentes a uma mesma estrutura definida pelo desenvolvedor, e assim, através do uso de caracteres específicos, pode indicar separações entre dados contidos em cada linha de texto.

Dessa forma, é possível elaborar um arquivo que contenha dados como nome, número de CPF e RG, data de nascimento e outros dados usando símbolos como “#” que não são comumente utilizados para separar os dados em cada linha, formando estruturas semelhantes às utilizadas em sistemas de bancos de dados simples.

Existe um trabalho padrão de manipulação de dados em estruturas de dados que, independentemente de serem ou não gravados com algum tipo de recurso de persistência de dados, servem para inserir dados e manipulá-los conhecido como CRUD (Create, Read, Update, Delete ou criação, consulta, atualização, exclusão de dados).

Estes processos básicos são essenciais para que se possam gerenciar dados de forma minimamente adequada, mas é possível adicionar funcionalidades extras como geração de relatórios, envio de dados pela *web*, conversão de dados, etc.

Para fins de estudo em algoritmos que não geram ainda produtos para mercado e se propõem apenas a introduzir os conceitos fundamentais da programação neste momento dos estudos, fica como proposta para pesquisas e estudos futuros com aplicação em linguagens de programação comerciais.

Para compreender como é estruturado um algoritmo para manipulação de dados em arquivos do tipo texto, observe o exemplo da imagem 46 para compreender o que é agregado ao que já foi estudado anteriormente.

TIPO CADASTRO = REGISTRO

INTEIRO: CODIGO, IDADE;

CARACTERE: NOME, ENDEREÇO, CIDADE, ESTADO

FIMREGISTRO;

TIPO ARQ = ARQUIVO COMPOSTO DE CADASTRO;

CADASTRO: DADOS;

ARQ: AGENDA

Imagem 46. | Fonte: O autor.

Neste exemplo da imagem 46 é possível reconhecer a declaração de uma estrutura de dados heterogênea como já estudado. O registro nomeado de “CADASTRO” possui campos que podem ser preenchidos com dados do tipo texto, podendo, se necessário, ser adicionados a um arquivo de dados.

Uma nova instrução utilizada na manipulação de arquivos inicia com a palavra reservada “TIPO”, seguida de um nome arbitrário “ARQ”, e depois, o símbolo “=” com o complemento informando que a estrutura se refere a uma arquivo de dados baseado na estrutura “CADASTRO” declarada anteriormente.

Depois, uma variável com o nome “DADOS” é declarada com o tipo “CADASTRO” para a manipulação de dados, assim como outra variável “AGENDA” é declarada com base no tipo “ARQ” declarado para manipulação de arquivos.

Importante ressaltar que não é obrigatório o uso de estruturas de dados do tipo registro para armazenamento de dados em arquivos, pois os dados podem ser estruturados em variáveis simples do tipo “CARACTERE” tendo em mente que a organização de mais de um dado por linha do arquivo teria que ser organizada de forma manual na variável.

É importante ter em mente que os arquivos geralmente possuem nome e extensão, sendo que a extensão auxilia na identificação do *software* que utiliza cada arquivo, e assim, é interessante que se conheçam extensões mais comuns para que não sejam utilizadas na criação de arquivos de dados para algoritmos criados.

Acesse o link:[Disponível aqui](https://support.microsoft.com/pt-br/help/4479981/windows-10-common-file-name-extensions)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

Existem palavras reservadas próprias para a manipulação de arquivos de texto segundo Forbellone (2005) que necessitam de alguns parâmetros como a indicação do arquivo a ser manipulado. Observe os comandos na imagem 63 para conhecer como são estruturadas instruções com estas palavras reservadas.

ABRA (AGENDA);

AVANCE (AGENDA);

GUARDE (AGENDA, DADOS);

COPIE (AGENDA, DADOS);

FECHE (AGENDA);

ELIMINE (AGENDA);

Imagem 46: Instruções para manipulação de arquivos. | Fonte: O autor.

Nos exemplos de instruções contidos na imagem 46 temos primeiramente uma instrução utilizada para se abrir arquivos de texto com a palavra reservada “ABRA” que necessita que o arquivo seja informado, e no caso do exemplo, a variável “AGENDA” é responsável por conter o arquivo a ser manipulado na execução do algoritmo.

A instrução composta pela palavra reservada “AVANCE” e pelo parâmetro “AGENDA” fazem com que um índice de navegação pelo arquivo avance até uma próxima linha e permita que os dados desta linha sejam manipulados.

Outra instrução apresentada no exemplo utiliza a palavra reservada “GUARDE” para realizar a ação de armazenar fisicamente os dados contidos na variável “DADOS” na próxima linha do arquivo texto indicado por “AGENDA”.

Na sequência, a instrução definida pela palavra reservada “COPIE” traz do arquivo texto, cópias dos dados contidos para que possam ser inseridos na variável “DADOS” e possam ser utilizados pelo algoritmo, e possam, se necessário, serem novamente gravados em disco.

A instrução utilizando a palavra reservada “FECHE” apenas possui a função de encerrar o uso do arquivo indicado por “AGENDA” para reduzir as chances de os dados serem corrompidos em função do arquivo de se manter aberto sem necessidade.

Por fim, a última instrução do exemplo da imagem 63 traz uma instrução que utiliza a palavra reservada “ELIMINE” para excluir todo o arquivo indicado por “AGENDA” tendo ou não dados inseridos no mesmo, e por isto, deve ser utilizado com máximo cuidado.

Imaginar aplicações desenvolvidas para manipular estruturas de dados heterogêneas em quantidade não pré-estabelecida é um bom tipo de utilidade para o uso de arquivos de texto.

Estes arquivos podem conter grandes quantidades de linhas, e cada linha pode conter os dados de uma estrutura heterogênea organizados de forma a um separador destacar o início e fim de cada dado na linha.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

Para finalizar os estudos, um exemplo completo de algoritmo para inclusão de dados em um arquivo de dados para demonstração do uso de instruções próprias para manipulação de arquivos texto:

INÍCIO

DECLARE

TIPO DADOS = REGISTRO

CARACTERE: NOME;

INTEIRO: TELEFONE;

FIMREGISTRO;

TIPO ARQUIVO = ARQUIVO COMPOSTO DE DADOS;

DADOS: REGISTRO;

ARQUIVO: AGENDA;

ABRA (AGENDA);

REPITA

AVANCE (AGENDA);

ATÉ FDA (AGENDA);

LEIA (REGISTRO.NOME);

LEIA (REGISTRO.TELEFONE);

GUARDE (AGENDA, REGISTRO);

FECHE (AGENDA);

FIM.

Imagem 47: Exemplo de algoritmo para manipulação de arquivos. | Fonte: Adaptado de Forbellone (2005).

Neste exemplo de algoritmo da imagem 47, é declarado um registro para armazenamento temporário de dados a serem incluídos posteriormente em arquivo de dados. Para isto, um laço de repetição realiza o avanço até o final do arquivo para que novos dados sejam adicionados após o último registro previamente gravado.

Depois, é realizada a leitura de dados para o registro de forma que os dois campos sejam preenchidos pelo usuário e depois gravados em disco com o comando “GUARDE” e, ao final, o arquivo seja devidamente fechado para garantir a correta gravação dos dados e integridade do arquivo.

A manipulação de arquivos de texto é bastante útil e pode agregar uma grande quantidade de outros conceitos estudados ao longo do material como estruturas de controle de fluxo de execução, e por isto, uma boa forma de se praticar é elaborar algoritmos que gerem dados de tipos variados e que sejam depois armazenados em disco.

O exemplo da imagem 65 é um exemplo de dados que está guardado em um arquivo indicado pela variável “AGENDA” e que através de uma estrutura de repetição “REPITA” busca dados em sequência do arquivo para uma estrutura de dados homogênea (vetor) declarada com um tipo de dados heterogêneos (registro).

Um detalhe a ser observado é que a estrutura de repetição é controlada pelo avanço nas linhas do arquivo com o comando “AVANCE” e encerra as iterações quando o final do arquivo é atingido com a palavra reservada “FDA” no comando “ATÉ”.

TIPO DADOS = VETOR \[1..100\] DE CADASTRO;

DADOS: LISTA; INTEIRO: I;

ABRA (AGENDA);

REPITA

AVANCE (AGENDA);

COPIE (AGENDA, LISTA \[I\]);

I <- I + 1;

ATÉ FDA (AGENDA);

Imagem 48: Exemplo para leitura de dados em arquivos. | Fonte: O autor.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Manipulação de Arquivos de Texto

Para complementar seus estudos, assista à videoaula a seguir: