---
title: "Classificação de Algoritmos"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-02.html"
author:
published:
created: 2026-05-07
description:
tags:
  - "clippings"
---
Classificação de Algoritmos

Disciplina: Algoritmo e Lógica de Programação
Aula 2 - Classificação de Algoritmos

Sumário

Algoritmos são aparentemente simples por utilizarem idioma comum e não necessitar de ferramenta alguma além de um editor de textos simples para ser escrito, além do que pode também ser escrito à mão, pois seu intuito é de propor ideias e soluções, mas não de programá-las.

Por esta característica, o nível de detalhamento dos processos pode ser baixo e apenas as principais ideias serem colocadas na elaboração, pois a codificação em alguma linguagem de programação precisa ser detalhada o suficiente para implementar todos os requisitos necessários e demais elementos de forma a compor um *software* que seja funcional e atenda às expectativas do cliente.

Geralmente, a ideia na concepção de um algoritmo é que seu pseudocódigo seja estruturado de forma que a execução das instruções seja realizada da mesma forma que a leitura de uma página de texto, de forma sequencial, desde o início até o fim da página. Observe a imagem 5 para que se tenha uma ideia da estrutura de um algoritmo com instruções sequenciais.

INÍCIO

ESTRUTURAS DE DADOS;

INSTRUÇÃO;

INSTRUÇÃO;

...

INSTRUÇÃO;

FIM.

Imagem 5: Exemplo de estrutura de algoritmo imperativo | Fonte: O autor.

Neste exemplo da figura 5, a estrutura do algoritmo inicia por uma palavra reservada **INÍCIO**, tendo em seguida a declaração das estruturas de dados a serem utilizadas no mesmo.

Em seguida, inicia-se uma sequência variável de instruções a serem executadas sequencialmente no algoritmo, podendo estas ser responsáveis por ações de entrada ou saída de dados, e pelo processamento destes dados dentro da proposta de funcionalidade do algoritmo.

Esta forma sequencial e seriada de execução de algoritmos, por ser a mais comum, também acaba sendo a mais indicada para iniciantes, pois além de uma lógica mais simples de compreensão, também contém muito mais conteúdo em meios de pesquisa como livros e a *web*.

Os chamados paradigmas de linguagens de programação que representam formas distintas de programação possuem também maneiras de serem representados em forma de algoritmo, pois esta representação usando pseudocódigo é limitada apenas pela capacidade criativa de quem propõe soluções utilizando este recurso.

Esta forma sequencial de escrita de pseudocódigos está relacionada com um paradigma chamado imperativo que predomina a construção de código de forma sequencial do início ao final de um código, utilizando apenas as estruturas básicas da linguagem ou neste caso, do pseudocódigo para a implementação.

Outro tipo de algoritmo é constituído por partes parcialmente independentes de pseudocódigos estruturados em forma de sub-rotinas que servem para que um algoritmo seja composto por partes independentes entre si de preferência, e que possam se comunicar de forma integrada, oferecer uma solução computacional completa que aparentemente é executada como um algoritmo sequencial.

Os algoritmos podem ser inseridos em uma segunda categoria de paradigmas de programação chamados de estruturados por permitirem a subdivisão de um pseudocódigo em partes que possam se comunicar por meio da troca de dados entre estas sub-rotinas. Observe a imagem 6 para um exemplo de estrutura de algoritmo estruturado.

PROCEDIMENTO TESTE()

INÍCIO

INSTRUÇÃO;

...

INSTRUÇÃO;

FIM.

INÍCIO

INSTRUÇÃO;

...

TESTE();

...

INSTRUÇÃO;

FIM.

Imagem 6: Exemplo de estrutura de algoritmo estruturado | Fonte: O autor.

No exemplo da imagem 8, ao invés de iniciar o algoritmo pela palavra reservada **INÍCIO** como de costume, utiliza-se a palavra reservada **PROCEDIMENTO** para indicar o início de uma sub-rotina chamada **TESTE()** que contém instruções para alguma finalidade específica e que pode ser chamada a qualquer momento pelo trecho principal de pseudocódigo do algoritmo.

A parte principal do algoritmo que é por onde inicia sua execução possui instruções normais após a palavra reservada **INÍCIO**, mas em determinado momento, chama o procedimento **TESTE()** para que este realize um procedimento necessário para a sequência da execução do código.

Esta divisão do algoritmo em parte principal e sub-rotina contendo diferentes trechos de pseudocódigo são a base da programação estruturada, e esta é uma das formas mais utilizadas de programação no mercado.

Compreender a estrutura de um algoritmo ou código de uma linguagem de programação é o primeiro passo essencial para se aprender a programar, mas antes ainda, é preciso aprender a interpretar problemas e deles obter informações capazes de auxiliar no início do esboço da lógica de uma provável solução computacional.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

Existem algoritmos que tratam de uma lógica mais complexa e evoluída do uso de sub-rotinas capazes de chamar a si mesmas de forma iterativa ou repetitiva, também chamada de recursiva, em que existe um controle da quantidade de iterações baseado em uma condição que muitas vezes envolve valores numéricos que ao serem atingidos, encerram as sucessivas chamadas à sub-rotina e às seguidas repetições.

O paradigma estruturado citado anteriormente permite uso desta técnica, mas há outros paradigmas que permitem uso deste recurso no desenvolvimento de *software* como o paradigma funcional e o paradigma orientado a objetos.

Esses paradigmas representam maneiras mais específicas e de lógica mais complexa para elaboração de algoritmos e não são as formas mais populares de uso. Este tipo de recurso para lidar com sub-rotinas será melhor detalhado mais adiante em uma aula posterior.

Praticar programação não representa apenas digitar códigos prontos e executá-los. Realizar ajustes quando erros ocorrem de forma a demonstrar que a lógica da solução é compreendida e a sintaxe do pseudocódigo ou linguagem de programação é compreendida, representa que se possui preparo e raciocínio lógico necessários para o correto desenvolvimento de uma solução para um problema.

Se esta solução é escrita da maneira mais correta ou eficiente, isto depende muito da complexidade da solução e experiência em programação do desenvolvedor, mas isto se alcança com a experiência de desenvolver *softwares* variados.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-abordagem-center.svg)

Um outro paradigma chamado de funcional se baseia em sub-rotinas que executam processos como se fossem funções matemáticas em que se evita, ao máximo, mudanças de estado ou dados dinâmicos que são características comuns nos paradigmas imperativo e estruturado que utilizam muitas estruturas de dados variáveis e estados que mudam o tempo todo na execução.

Por ser uma forma de programação mais específica e não tradicional será deixada de lado neste material, sabendo que sua relevância está aumentando em diversas linguagens de programação, devido a algumas características deste paradigma, como facilidade na estruturação da semântica de seus códigos, e por serem linguagens com uma escrita bem específica e compacta, facilita a busca por erros quando necessário.

Outro paradigma bastante popular é chamado de orientação a objetos e possui pontos em comum com a programação estruturada, mas com diferenciais em sua metodologia que diferenciam os paradigmas como a chamada abstração que converte problemas reais em classes que possuem as principais características do problema e as soluções computacionais são estruturas semelhantes a sub-rotinas com uma maior independência que no paradigma estruturado.

Esta forma de programação cria códigos mais independentes entre si e que podem ser integrados com certa facilidade, devido a uma característica do paradigma que busca tornar seus componentes independentes ao máximo para que seja mais bem realizado o chamado reuso de código. Observe o exemplo da imagem 7 para um auxílio nos estudos deste paradigma.

CLASSE EXEMPLO

ATRIBUTO DADO;

...

MÉTODO PROCESSA();

...

EXEMPLO OBJ;

Imagem 7: Exemplo de estrutura de algoritmo orientado a objetos | Fonte: O autor.

Neste exemplo contendo um trecho de pseudocódigo baseado na ideia de programação orientada a objetos, uma classe chamada EXEMPLO é declarada contendo um atributo DADO de exemplo, e um método PROCESSA() funcionando ambos de forma semelhante a variáveis e funções, mas de forma diferente, seguindo os princípios desse paradigma.

Neste pseudocódigo, exemplo da imagem 9, algumas palavras reservadas foram utilizadas, e foram definidas para este estudo como sem a utilização de algum padrão conhecido, e assim, as palavras CLASSE, ATRIBUTO e MÉTODO foram definidas para este material como representativas de elementos do paradigma de orientação a objetos.

Outra forma de se estruturar algoritmos se baseia em regras da lógica matemática para avaliar expressões usando dados imutáveis para obtenção de resultados verdadeiros ou falsos, ou para construção de novas regras a partir das existentes.

Este método de desenvolvimento de código é bastante específico e utilizado em poucas linguagens de programação para geração de *software* voltado para o desenvolvimento de sistemas especialistas que trabalham com relações entre dados para obter novas informações tendo influências da área de inteligência artificial no desenvolvimento deste paradigma.

Esses chamados paradigmas de programação são a base de todas as linguagens de programação, e há mais paradigmas diferentes existentes. Com o avanço da tecnologia da informação e o desenvolvimento de novos tipos de *software* para estas tecnologias, novos paradigmas também surgem para adequar a programação às novas necessidades.

Além dos paradigmas que representam diferentes formas de se elaborar *software* para resolução de problemas computacionais, existem as diferentes técnicas para se elaborar algoritmos que possuem suas características particulares e se adequam a tipos diferentes de problemas ou trazem formas diferentes para solucionar os mesmos problemas.

Uma forma de se solucionar problemas é fracioná-los em problemas menores, e esse fracionamento pode se repetir com as partes já reduzidas até que cada parte do problema seja simples o suficiente para ser facilmente resolvido e que uma solução possa ser desenvolvida, mantendo relação com as demais partes para que possam ser integradas posteriormente.

Um exemplo desta técnica seria, por exemplo, a separação de cada parte relativa a cada cálculo de um algoritmo de implementação de uma calculadora para que todas estas partes organizadas em estruturas chamadas de sub-rotinas, por exemplo, possam ser acessadas sempre que necessário pelo restante do pseudocódigo, mas mantendo-as como estruturas mais independentes dentro do algoritmo como um todo.

Algoritmos podem ser utilizados para resolver outros problemas, ou terem processamento realizado por um algoritmo reaproveitado em outro algoritmo para reduzir o uso de recursos e ganho de tempo e desempenho geral.

Existem algoritmos bastante específicos e até muito conhecidos para resolver problemas e subproblemas bastante comuns a problemas maiores como a ordenação de dados, a maximização ou minimização de resultados obtidos, processamento matemático ou físico, etc.

Algoritmos conhecidos como algoritmos de ordenação (*bubble sort, merge sort,* etc.), algoritmos de estruturas chamadas de grafos que se baseiam na ligação de pontos por arestas que podem ser aplicados a muitos problemas reais, etc.

Alguns algoritmos mais complexos envolvem heurística que representam soluções cognitivas e não racionais para processamento de escolhas mais rapidamente e ignorando detalhes que em outros tipos de algoritmos seriam relevantes.

Assim, os algoritmos que se baseiam nos tipos de funcionalidades devem possuir: problemas a resolver e técnicas a serem aplicadas em alguma linguagem baseada em um ou mais paradigmas de programação para gerar soluções computacionais para problemas reais.

Algoritmos podem ser simples e não necessitar de recursos muito específicos para resolver problemas lógicos complexos, ou precisar de recursos muito completos para atender demandas muito complexas e necessitar de muito mais tempo para serem implementados por completo.

  <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Classificação de Algoritmos

Para complementar seus estudos, assista à videoaula a seguir: