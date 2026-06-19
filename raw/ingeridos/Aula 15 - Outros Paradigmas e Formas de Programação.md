---
title: "Aula 15 - Outros Paradigmas e Formas de Programação"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-15.html"
author:
published:
created: 2026-06-18
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 15 - Outros Paradigmas e Formas de Programação

Sumário[1\. Programação Orientada a Eventos](#topico-01)[

2\. Programação Orientada a Aspectos

](#topico-02)[

3\. Programação Dinâmica

](#topico-03)

Além dos tradicionais quatro paradigmas tratados ao longo do material, existem alguns diferentes paradigmas que surgiram com base em um ou mais dos paradigmas tradicionais, ou apenas definições mais específicas para determinados tipos de programação utilizados para solucionar problemas específicos e necessidades pontuais.

## Programação Orientada a Eventos

Um paradigma alternativo existente é o **orientado a eventos,** que trata da interação de software com eventos esperados com base em rotinas de tratamento de gatilhos acionados por eventos do sistema como mecanismos de entrada, eventos de softwares em execução ou do sistema operacional, por exemplo.

Não é necessariamente uma extensão do paradigma orientado a objetos, mas pode utilizar conceitos deste paradigma, como ocorre com a linguagem C#, por exemplo.

Aceita o uso de recursos como *design* *patterns* que não representam códigos prontos para o desenvolvimento de softwares, mas modelos para auxiliar em problemas a partir de soluções já desenvolvidas, utilizadas e testadas.

Utilizado em aplicações que utilizam interfaces gráficas para interação com usuários, recebem estas interações como gatilhos para eventos e estes são tratados pelos códigos associados a estes eventos.

Eventos ocorrem em momentos que podem ser previsíveis ou não, envolvendo interação humana ou não, sendo representados por cliques, teclas apertadas, botões de controles, toques em tela sensíveis ao toque, e entradas de dados automatizadas, por exemplo.

Os eventos são monitorados e quando eventos esperados ocorrem podem tratados pelo software usando recursos do próprio sistema operacional, e quando eventos inesperados ocorrem, podem ser tratados diretamente pelo sistema operacional pelo fato de não serem tratados pelo software. Quanto mais completo o tratamento de eventos pelo software, mais completa e robusta é a aplicação.

As linguagens podem ter recursos específicos para o tratamento de eventos em forma de comandos nativos da linguagem, bibliotecas padrões da linguagem ou criadas pelos próprios desenvolvedores para atender necessidades pontuais, etc.

Aplicações para as áreas de bancos de dados, sistemas de arquivos, softwares compartilhados de rede, ferramentas para sistemas operacionais, tratamento de interrupções e aplicações comerciais onde eventos devam ser capturados e tratados.

A interface gráfica desenvolvida por muitos softwares para interação com usuários é um meio tipicamente orientado a eventos relacionados a cliques de mouse, por exemplo, sendo estes capturados primeiramente pelo sistema operacional e tratados pelo software de acordo com os objetos acionados e a forma como ocorre o clique do mouse (botão, arrasto, etc.).

Neste tipo de software, normalmente existe uma rotina que fica sendo executada por padrão e é interrompida por eventos para que haja o processamento relacionado ao tratamento destes eventos, mas depois, a rotina principal que aguarda eventos volta a funcionar a partir dos retornos das funções acionadas nos eventos.

Linguagens que geralmente criam soluções baseadas em interfaces gráficas como as versões Visual Basic, Visual C e Delphi que criam aplicações desktop tipicamente dotadas de interfaces gráficas são um bom exemplo, assim como linguagens como C#, Java e JavaScript que geralmente lidam com o tratamento de eventos em formulários web.

Esta forma de programação acaba tendo um fluxo de execução diferente dos paradigmas imperativo e orientado a objetos por não ter um fluxo contínuo determinado normalmente pelo próprio processamento de dados na aplicação, e sim pode eventos que ocorrem de forma inesperada pelo software normalmente, podendo inclusive, nunca ocorrer.

Muitas vezes, softwares embarcados em dispositivos IoT funcionam com base em laços de repetição infinitos que são interrompidos apenas por eventos ocorridos durante a execução ou interrupções de funcionamento, como ocorre em placas Arduino que recebem código em uma versão própria da linguagem C.

Imagem 1

**int azul = 13;**

**int vermelho = 14;**

**void setup() {**

**pinMode (azul, OUTPUT);**

**pinMode (vermelho, OUTPUT);**

**}**

**void loop() {**

**digitalWrite (azul, HIGH);**

**delay (100);**

**digitalWrite (vermelho, HIGH);**

**delay (100);**

**digitalWrite (azul, LOW);**

**delay (100);**

**digitalWrite (vermelho, LOW);**

**delay (100);**

**}**

O código presenta na imagem 1 traz um exemplo de software que pode ser embarcado em uma placa Arduino como a mostrada na imagem 63 que permite que códigos em linguagem C sejam inseridos no chip de memória da placa para serem executados assim que a placa seja carregada eletricamente.

Esse código traz um exemplo de aplicação da placa onde dois leds de cores azul e vermelho podem ser ligados nos pinos 13 e 14 respectivamente para que sejam acesos e apagados sequencialmente a cada período de tempo indicado na função delay().

O código é dividido em duas funções, sendo a função setup() responsável pelas configurações físicas da placa em relação ao código, e a função loop() o laço de repetição infinita que aguarda os possíveis eventos de interrupção do modo de espera da placa aguardando eventos.

Imagem 2

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a15-img01.jpg)

Fonte: Pixabay.

Interrupções de hardware como botões pressionados em um projeto Arduino ou interrupções de software como cliques geram tratamentos diferentes por parte do conjunto hardware, sistema operacional e software, e até interpretadores de comandos de linguagens interpretadas são exemplos de orientação a eventos, aguardando comandos do usuário.

Outra forma distinta de programação é feita por blocos de forma gráfica, bastante intuitiva e de facílima compreensão utilizada em linguagens como Scratch ou Blocky que oferecem objetos em formas apropriadas para encaixe uns com os outros de forma que comandos de repetição tenham um formato que sirva para englobar outros comandos, gerando instruções completas em blocos, e daí a ideia da programação em blocos.

Extremamente didáticas, essas linguagens se tornaram perfeitos métodos de inserção de pessoas de todas as idades no aprendizado de lógica de programação, oferecendo meios de compreender ludicamente, o desenvolvimento das principais estruturas de código geralmente associadas ao paradigma imperativo. Com uma sintaxe e semântica extremamente simples, mas completa, essas linguagens ganharam, espaço na área de educação e se tornaram propostas de método de programação para o futuro, onde algoritmos formados por blocos podem ser traduzidos em outras linguagens e gerar aplicações funcionais.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

## Programação Orientada a Aspectos

Outra forma de programação relevante é a relacionada ao chamado paradigma orientado a aspectos, em que é possível organizar o código a partir de sua relevância dentro dos requisitos e propósitos em cada aplicação, complementando o paradigma orientado a objetos que se baseiam em comportamentos de objetos, agindo como código auxiliar nas aplicações.

Paradigma desenvolvido por Gregor Kiczales e a sua equipe na Xerox PARC, a divisão de pesquisa da Xerox, serviu de base para o desenvolvimento de uma linguagem de programação orientada a aspectos chamada AspectJ que oferece mecanismos para que classes públicas comuns possam ser reorganizadas como classes em aspectos.

A linguagem AspectJ não cria aplicações completas, mas complementos para aplicações Java, assim como linguagens como PHP e JavaScript podem ser ligadas a scripts HTML e CSS para funcionarem conjuntamente.

Aspectos são organizações de partes de um código de acordo com seu nível de importância dentro de toda a aplicação, permitindo que haja um encapsulamento em módulos separados de código secundário, estrutura que não é contemplada pela linguagem Java, gerando mecanismos para controle transversal de código.

Um *aspect* *weaver* é uma ferramenta que age como um compilador, compondo uma aplicação completa que contém toda a parte fundamental do código em importância unida a todos os aspectos que contém códigos transversais de menor relevância através de um processo chamado *weaving*.

A imagem 2 traz um exemplo de aplicação de código conjunto Java e AspectJ separados em dois arquivos que são unificados no processo de compilação para geração de arquivo *bytecode* para interpretação pela máquina virtual Java como padrão da linguagem.

Imagem 2

// Arquivo Java - Mensagem.java

**public class Mensagem {**

**public static void entrega(String mensagem) {**

**System.out.println(mensagem);**

**}**

**public static void entrega(String person, String mensagem) {**

**System.out.print(person + ", " + mensagem);**

**}**

**}**

//Arquivo AspectJ - Aspecto.java

**public aspect Aspecto {**

**pointcut enviaMensagem()**

**: call( Mensagem.entrega("Mensagem enviada!"); );**

**before(): enviaMensagem () {**

**System.out.print("Testando... ");**

**}**

**}**

Fonte: Laddad (2003 - Adaptado).

O código do arquivo Java na imagem 2 existe um típico código em linguagem Java que simplesmente tem a função de exibir uma frase para o usuário e na sequência, no código do arquivo Aspecto.java, a declaração de um aspecto, onde ocorre a declaração do *pointcut*, uma espécie de desvio que contém o chamado *join* *point* que define a ligação entre classe e aspecto.

Recursos para controle de prioridades na execução são definidos através do uso da palavra reservada *before* que indica que o conteúdo do método enviaMensagem() desta linha deve ser executado antes do conteúdo do método enviaMensagem() principal indicado pelo *pointcut* *call* representando um desvio incondicional durante a execução como era feito com o uso de GOTO décadas atrás.

A adição deste mecanismo de aspecto faz com que a mensagem indicada por *before* no aspecto seja exibida antes da mensagem indicada pela palavra reservada *call* obtendo como resultado “Testando... Mensagem enviada!”, mostrando assim que mecanismos de tratamento de erros de abertura de arquivos ou tratamentos de erros diversos que são executados durante a execução normal da aplicação possam ser agrupados em forma de aspectos.

## Programação Dinâmica

Uma última forma de programação a ser estudada se chama programação dinâmica e permite que problemas complexos possam ser reduzidos a problemas de menos complexidade, de forma a obter otimização no processo de desenvolvimento de software.

Uma aplicação para este mecanismo é no uso da teoria de grafos aplicável em muitas soluções computacionais como de rotas logísticas, onde pontos de referência das rotas podem ser representados por vértices e os caminhos possíveis serem definidos por arestas que ligam pares de vértices e podem servir como base para avaliação de menores caminhos ou que agreguem menores ou maiores custos de forma geral.

Imagem 3

Ponto A ----------- Ponto B ----------- Ponto C ----------- Ponto D

Ponto C ----------- Ponto A ----------- Ponto D

Uma estrutura como a mostrada na imagem 3 que pode também de representada em forma de diagrama ou como uma estrutura de dados do tipo vetor ou matriz, é uma aplicação para a programação dinâmica.

As relações entre os pontos podem ser definidas apenas por serem adjacentes, ou seja, vizinhos como o Ponto A e o Ponto B, mas podem ser agregar valores chamados de pesos que influenciam diversas situações tais como na escolha dos algoritmos adequados para buscar as melhores rotas.

Conhecer os conceitos básicos da teoria de grafos é bastante relevante para estudos na área de TI e deve fazer parte dos conhecimentos essenciais de desenvolvedores de soluções computacionais.

Fonte:[Disponível aqui](https://medium.com/xp-inc/grafos-teoria-e-aplica%C3%A7%C3%B5es-2a87444df855)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

Uma característica importante da programação dinâmica é a possibilidade de estruturação de problemas de otimização de etapas a serem resolvidas sequencialmente, considerando os problemas fracionados como completos, desde que seja possível a integração das partes como uma solução completa para o problema original.

Problemas como de controle de estoque pode ser considerado como problema dinâmico, principalmente no comércio eletrônico onde o processo de movimentação do estoque é mais rápido e podendo ter uma complexidade maior que estoques físicos.

Uma entrada de dados pode servir como base para o processamento realizado pelo programa, sendo decisiva para como o processamento deve ser realizado, e como pode depender de vários aspectos para que os processos sejam realizados, sua previsibilidade se torna fraca e o software necessita então ser capaz de se adaptar a eventos.

Alguns problemas como no caso dos softwares de rota para GPS precisam ser dinâmicos, pois seus cálculos podem ser influenciados a todo instante por fatores inesperados como acidentes, obras ou o simples caso de o motorista se equivocar nos comandos dados pelo software.

Na otimização, os estados do processo se referem ao que é necessário para que o software possa realizar seus processos adequadamente de acordo com a dinâmica dos eventos que podem ocorrer inesperadamente ou de forma previsível, observando impactos nos processos realizados e retornos gerados.

Algumas características que auxiliam na determinação dos estados são relativas a o método com o qual os estados são obtidos não deve afetar a tomada de decisão sobre como ocorrem as transmissões de dados nos estados.

A linguagem Clojure é uma linguagem que aceita programação dinâmica, e mesmo sendo tipada, durante o processo de compilação de seus códigos, os tipos não são verificados, e como as estruturas de dados em Clojure são listas geralmente, podendo ser manipuladas em tempo de execução pode-se interferir nas funcionalidades do código em tempo real.

 <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Programação Orientada a Eventos
- Programação Orientada a Aspectos
- Programação Dinâmica

Para complementar seus estudos, assista à videoaula a seguir: