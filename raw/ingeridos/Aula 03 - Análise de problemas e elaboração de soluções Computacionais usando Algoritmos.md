---
title: "Aula 03 - Análise de problemas e elaboração de soluções Computacionais usando Algoritmos"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-03.html"
author:
published:
created: 2026-05-28
description:
tags:
  - "raw"
---
Disciplina: Algoritmos e Lógica de Programação
Aula 03 - Análise de problemas e elaboração de soluções Computacionais usando Algoritmos

Sumário[1\. Introdução](#topico-01)[

2\. Codificação e Execução de Programas

](#topico-02)

Problemas são a razão de serem desenvolvidos os algoritmos. Desde problemas menos complexos como um cálculo pequeno ou uma simples entrada e saída de dados com o mínimo de processamento, até sistemas complexos compostos de vários módulos que realizam processamento de grandes volumes de dados ou atividades complexas como jogos, cálculos avançados, etc.

Algoritmos representam meios de se programar dispositivos diversos que podem ser simples como autômatos mecânicos programáveis e circuitos elétricos simples ou dispositivos mais complexos que possuam sistemas operacionais sendo executados e que sobre eles sejam executados os demais *softwares* desenvolvidos a partir de algoritmos.

A programação de autômatos foi uma das formas de se materializar a teoria das linguagens formais desenvolvida na década de 1950, e que permitiu o desenvolvimento de aplicações baseadas em análise léxica e sintática para o desenvolvimento de linguagens artificiais precursoras das linguagens de programação utilizadas até os dias de hoje.

Acesse o link:[Disponível aqui](https://autociencia.blogspot.com/2018/08/linguagens-formais-automatos.html)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

A ideia de todo *software* desenvolvido a partir de um algoritmo é a de realizar uma série de passos para solucionar problemas, atendendo a requisitos definidos como necessários para que o *software* seja considerado adequado e realmente funcional, pois não basta apenas um *software* ser funcional sem realizar o que dele se espera.

Há *software* que é desenvolvido especificamente para determinado *hardware* e com finalidade bastante específica desde o princípio quando Ada Lovelace (Augusta Ada King, Condessa de Lovelace), matemática e escritora inglesa, que na década de 1840 traduziu um artigo de um engenheiro militar italiano. Também escreveu anotações adicionais que foram consideradas o primeiro programa de computador da história.

Com a evolução do *hardware*, e a expansão do que era possível realizar com as diversas variações do mesmo, o desenvolvimento de *software* para estes também foi sendo modificado e toda uma nova indústria surgiu para atender à demanda crescente de desenvolvimento de *software*. Desde a grande expansão tecnológica ocorrida em função da maior popularização do *hardware* proporcionada por empresas como a IBM e Apple, que desenvolveram equipamentos com bom desempenho, com tamanho e preço acessíveis a partir da década de 1980 quando surgiu o computador pessoal principalmente.

Assim, com equipamentos cada vez mais potentes e menos específicos, o *software* passou por grandes mudanças e com o surgimento dos sistemas operacionais capazes de serem executados nesses computadores de propósito geral, o desenvolvimento de *software* passou a um nível mais alto em que não era mais primordial que o *software* conversasse com o *hardware* diretamente, e sim, com o sistema operacional encarregado da intermediação desta interação.

Da mesma forma que o *hardware* foi sendo inserido em todas as atividades humanas, desde a indústria até o lazer, foi sendo então desenvolvido *software* para atender a toda esta nova demanda de produtos que permitissem que computadores com sistemas operacionais instalados pudessem ser utilizados para facilitar e automatizar tarefas antes realizadas apenas de forma manual ou mecânica.

Imagem Ilustrativa.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a03-img1.jpg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg) ![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/icon-seta.svg)

Uma mudança importante que ocorreu foi uma adaptação dos programadores e linguagens de programação aos sistemas operacionais, pois estes passaram de uma interface totalmente textual e monocromática ao uso de cores num primeiro momento e unidades de discos magnéticos muito mais eficientes e rápidos em relação ao uso de rolos de fita ou cartões perfurados, além de quantidades maiores de memória temporária para permitir a execução de *softwares* mais complexos.

Isto já gerou muitas mudanças na forma como se desenvolvia *software* e permitiu aplicações com maior complexidade computacional, pacotes de funcionalidades como o editor de textos Microsoft Word, desenvolvido na década de 1980 ou jogos que iniciaram uma nova era com evoluções muito rápidas em sua complexidade, em comparação aos existentes antes dos computadores pessoais.

Outra mudança impactante no desenvolvimento de *software* ocorreu com o desenvolvimento de interfaces gráficas para os principais sistemas operacionais existentes como os desenvolvidos por Apple, primeiramente, e Microsoft logo em seguida, por exemplo.

Já se pensava em interfaces gráficas para usuário (GUI) desde décadas anteriores como a desenvolvida pela XEROX, na década de 1970, mas com a Apple, na década de 1980, houve uma grande evolução do projeto original da XEROX usando um dispositivo apontador que foi implementado para uso nos computadores Lisa e Macintosh.

A GUI para o sistema MS-DOS surgiu em 1985 e se popularizou, na década de 1990, com as versões 3.0 e 3.11 que revolucionaram o mercado de computadores pessoais, antes dominado pela Apple, mas que passou a ter os computadores da IBM com sistema operacional MS-DOS e GUI Windows como um forte concorrente.

O desenvolvimento de *software* passou a ser voltado em grande parte, a produtos que se baseassem nestas interfaces gráficas, abrindo novos nichos de mercado e permitindo uma explosão de empresas de desenvolvimento e elevando a inserção da informática em todas as áreas de mercado e nos lares por todo o mundo em uma velocidade maior.

*Softwares* para jogos e aplicações comerciais começaram a ser produzidos em uma escala maior, permitindo que muitas empresas, novas no mercado, surgissem e outras, já mais estabilizadas, se tornassem verdadeiros gigantes na tecnologia.

Os computadores e sua infinidade de *softwares* desenvolvidos para aplicações diversas se tornaram importantes no processo de melhoria dos processos.

## Codificação e Execução de Programas

O processo de produção de *software* envolve uma série de etapas, desde a chamada modelagem de *software,* que trata dos contatos iniciais da elaboração de uma solução computacional para problemas, até a documentação inicial a que a solução se propõe a ter de funcionalidades para atender às demandas solicitadas.

Uma das formas de se desenvolver código em linguagens de programação se baseia na ideia de que o código deve ser pensado de forma que sua execução seja baseada num seguimento de instruções que vão sendo sequencialmente executadas de forma direta por um *software* encarregado de ler cada instrução e executar as instruções de forma direta sem que nenhuma conversão intermediária seja necessária no processo de execução do código fonte digitado.

Assim, para que seja possível a execução de programas de forma interpretada, é necessário que este programa seja digitado em forma de texto simples e gravado da forma adequada.

Depois, é necessário que a plataforma em que o mesmo será executado contenha um *software* para interpretação que pode ser próprio para tal função, como ocorre em navegadores para *Internet* que são criados para interpretar páginas *web* escritas em linguagem de marcação HTML.

Sem este *software* intermediário, o sistema operacional em si não contém recursos próprios para interpretação de programas diretamente, pois há muitas linguagens de programação variadas e a intenção do sistema operacional, quando instalado em um *hardware*, é de conter apenas recursos necessários para disponibilização das funcionalidades dos dispositivos de *hardware* aos usuários e algumas ferramentas básicas adicionais.

Outro tipo de linguagem de programação possui uma etapa intermediária de tradução de código em linguagem de programação para algo mais próximo da compreensão da máquina e excluindo elementos desnecessários para gerar um arquivo temporário necessário para uma segunda conversão.

Imagem Ilustrativa

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/a03-img2.jpg)

Esta segunda conversão gera um *software* executável a partir do arquivo temporário gerado chamado de arquivo objeto e não é utilizado posteriormente na execução. Apenas o *software* gerado pela segunda conversão é considerado *software* mesmo e pode então sem executado sem dependência com os dois arquivos da etapa anterior de código fonte e objeto.

Este método é empregado por todas as linguagens que utilizam o chamado compilador para a realização deste processo de tradução, e muitas linguagens se baseiam neste método para gerarem *software* com bom desempenho, que possam ser executados independentemente de outros *softwares* como em linguagens interpretadas.

Um ponto importante é que existem diferentes compiladores para as diferentes plataformas de *software* compatíveis com a linguagem de programação, e assim, para se executar um mesmo programa em várias plataformas é preciso que exista um compilador adequado a cada plataforma em que se deseja executar o *software*.

Caso um sistema operacional não possua um compilador para determinada linguagem de programação, *softwares* desta linguagem não seriam compatíveis com o sistema operacional por não haver meios para se gerar *softwares* executáveis para este sistema. Linguagens como C funcionam desta forma.

Um terceiro meio de se desenvolver programas para algumas linguagens de programação é utilizar um método híbrido dos dois anteriores em que um código é escrito normalmente em um editor e um arquivo contendo o código digitado é gerado.

Depois, um *software* compilador gera um arquivo intermediário objeto que não pode ser executado diretamente, mas sim, interpretado em um outro *software* interpretador que se baseia então no arquivo intermediário e não no código digitado diretamente.

Este *software* interpretador não gera *software* executável, mas apenas executa as instruções do programa, e por este motivo, necessita estar instalado e ser compatível com o sistema operacional desejado.

Assim, neste terceiro tipo de processo de execução de código, é preciso ter um arquivo texto com o código, utilizar um compilador para gerar um arquivo intermediário que pode então servir de base para um interpretador que então realiza a execução do *software*.

Neste caso são necessários dois *softwares* para a execução de outro, e por isto, uma tendência é um tempo maior para a execução de um *software* criado como acontece em linguagens como Java que possui boas qualidades e recursos, mas que possui este ponto negativo em relação ao seu desempenho geral em relação a algumas outras linguagens.

Avaliando as diferentes formas de se executar um *software*, é possível compreender que há fatores que tornam uma linguagem de programação mais atrativa ou indicada de acordo com os tipos de problemas a serem resolvidos, mas existe também a influência de como deve ser executado o *software*, seja de forma interpretada, compilada ou híbrida.

  <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Introdução
- Codificação e Execução de Programas

Para complementar seus estudos, assista à videoaula a seguir: