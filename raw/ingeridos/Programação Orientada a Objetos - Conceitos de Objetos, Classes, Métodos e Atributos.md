---
title: Aula 06 - Programação Orientada a Objetos - Conceitos de Objetos, Classes, Métodos e Atributos
source: https://ead.unimar.br/aulas/linguagens-de-programacao/aula-06.html
author:
published:
created: 2026-05-11
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 06 - Programação Orientada a Objetos - Conceitos de Objetos, Classes, Métodos e Atributos

Sumário[1\. Abstração](#topico-01)[

2\. Conceitos de Classe, Atributo, Método e Objeto

](#topico-02)

Mudando de paradigma de programação, iniciam-se os estudos do paradigma favorito do mercado atualmente, em que as soluções tendem a ser mais reutilizáveis, as abstrações de problemas a serem resolvidos organizadas em estruturas chamadas de **classes**, contendo características similares às da programação estruturada, mas trazendo novos conceitos que permitem algumas vantagens em relação ao paradigma estruturado.

## Abstração

A base para o paradigma orientado a objetos é a abstração de problemas em modelos instanciáveis chamados de **classes,** que agrupam propriedades e ações necessárias ao desenvolvimento de uma solução computacional para um problema.

Para entender um pouco da ideia da abstração, é interessante o uso de um exemplo prático: imagine consultório veterinário em que animais representam o foco do negócio, e ao redor dos animais orbitam produtos e serviços.

A abstração pode ser utilizada para iniciar uma proposta de solução para um software que resolva algumas ou várias demandas desse negócio, e é o ponto de partida para o desenvolvimento de software com base no paradigma orientado a objetos.

Em um negócio do tipo citado, é importante avaliar o que é necessário ser trazido de um problema controlado manualmente para um problema que seja controlado via software, e então é preciso compreender o chamado escopo do problema.

Digamos que nesse caso é solicitado que um software seja capaz de cadastrar animais com dados de identificação dele e de seus donos, além de serviços realizáveis e histórico de realização mais o controle de produtos para uso ou comercialização, por exemplo.

Assim, num primeiro momento, são identificadas as principais partes do problema para que delas sejam abstraídas estruturas de dados representativas de propriedades relacionadas ao problema, e depois sejam pensados os meios para se processar os dados.

Ao abstrair as propriedades necessárias para se implementar uma solução computacional, muitos aspectos devem ser levados em consideração, e a base da manipulação de dados é muito parecida com as utilizadas na programação estruturada.

Essas propriedades, chamadas de **atributos** na programação orientada a objetos, são equivalentes a campos em estruturas do tipo registro na programação estruturada, tanto é que este conceito não é utilizado na programação orientada a objetos, pois a classe é uma evolução dos registros.

Os registros da programação estruturada são estruturas de dados mais evoluídas que vetores, ou matrizes, porque permitirem dados de tipos diferentes agrupados, funcionando como tipos especiais vinculáveis a variáveis.

No caso do veterinário, na programação estruturada, seria criado um tipo registro (*struct* em linguagem C, por exemplo) que poderia ser nomeado “animais”, contendo definições de campos para armazenar as características dos animais que sejam relevantes para o negócio como nome, raça, data de nascimento, cor, peso, etc., além dos dados do dono, mas que poderiam estar armazenados em outra estrutura de registro para dados pessoais.

Um detalhe dos registros é que como sua declaração funciona como a criação de um tipo definido pelo usuário, esses devem servir como tipos para a declaração de estruturas de dados como variáveis, por exemplo.

Mas um registro armazena dados referentes a uma ocorrência apenas (animal, cliente) quando usado para declaração de uma variável, mas se usado como tipo para declaração de vetores, pode armazenar um registro de dados por unidade do vetor, funcionando sob o mesmo princípio dos bancos de dados.

Assim, existe a possibilidade de se criar estruturas como vetores definidas a partir de estruturas de registros para que se possa trabalhar com maiores volumes de dados em memória, mas ainda é possível utilizar as estruturas de registros para organizar dados que possam ser armazenados em arquivos do tipo texto, onde cada linha do arquivo pode armazenar um registro completo, por exemplo.

Fonte: Freepik.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a06-img01.jpg)

## Conceitos de Classe, Atributo, Método e Objeto

A organização da abstração do real para uma solução computacional é organizada em quatro elementos principais no paradigma orientado a objetos: classes, atributos, métodos e objetos.

No caso do paradigma orientado a objetos, os registros são substituídos por classes que, assim como os registros podem estar associados a dados heterogêneos armazenáveis em atributos ao invés de campos.

As classes são responsáveis por estruturar os softwares no paradigma orientado a objetos e dentro de uma classe, pode ser estruturada toda uma solução computacional, ou esta solução ser dividida em mais de uma classe dependendo de como é elaborada a abstração do problema real e sua complexidade.

Os chamados tipos de dados são fundamentais na maioria das linguagens de programação. Geralmente, uma linguagem de programação possui ao menos um tipo numérico de ponto flutuante para trabalhar com valores com a possibilidade de terem dígitos decimais, assim como podem ter tipos destinados apenas a valores inteiros.

Tipos de dados para caracteres e texto também são importantes, e muitas linguagens possuem um tipo próprio para valores lógicos ou booleanos verdadeiro e falso, mas também é possível utilizar números inteiros 1 e 0 para representar estes valores booleanos.

Esses tipos de dados são utilizados para a criação de variáveis em praticamente todas as linguagens de programação, e no paradigma orientado a objetos, geralmente são também utilizados para definir tipos para atributos de classes, indicando os tipos de dados utilizados para representar as propriedades destas classes.

Os atributos de uma classe se parecem em alguns aspectos como variáveis, mas sua finalidade e formas de uso são distintas, mesmo podendo geralmente representar unidades de dados com um tipo definido em sua implementação, pois variáveis são de propósito geral em termos de armazenamento de dados como valores recebidos pelo software, variáveis contadoras para laços de repetição, etc.

Os atributos se referem a propriedades em classes escolhidas para representar as características de elementos reais que foram abstraídas para a modelagem de classes que simulam estes objetos reais.

Os atributos são utilizados para armazenar dados referentes a um elemento específico obtido a partir de uma instanciação de classe para que os dados de atributos que caracterizam esta instância possam ser inseridos e processados como devido pelo software.

Essa instanciação de uma classe para que um elemento possa ser devidamente criado e utilizado como estrutura de dados e comportamentos relacionados a estes dados, recebendo o nome de objeto.

Objetos são então instâncias particulares de classes que representam elementos únicos com suas características próprias, sendo que uma classe pode servir como base para a geração de inúmeros objetos.

As classes não armazenam dados em si, servindo apenas como modelo para objetos que armazenam em cada instância, um conjunto particular de dados em atributos que podem ser então manipulados pelo software.

Esta manipulação é realizada por estruturas semelhantes às sub-rotinas chamadas de métodos que são responsáveis por realizar todo o processamento de dados de objetos de forma a serem essenciais para a implementação de software.

Os métodos representam ações que podem ser realizadas com atributos de forma a manipular seus dados e atender às funcionalidades definidas em requisitos do software e uma classe pode conter de zero a muitos métodos, sendo que estes métodos devem sempre ter relação direta com as classes e seus atributos de forma a afetar diretamente métodos instanciados.

Existe um recurso importante do paradigma orientado a objetos que está ligado à instância de objetos, tanto no momento de sua instanciação quanto de sua exclusão. O chamado **método construtor** possui o mesmo nome da classe à qual pertence, e é responsável por inicializar atributos com valores para o novo objeto, de forma a garantir que sejam criados com os dados adequados, de acordo com as necessidades de cada software. No momento em que é finalizado o uso de um objeto, um método destruidor (destrutor) com o nome da classe tendo um caractere diferenciador no nome como ~ antes do nome e servindo para a definição de elementos a serem descartados na memória, por exemplo.

Assim, uma classe Animais teria um método construtor Animais() para inicialização de dados e um destrutor com nome ~Animais() para liberar recursos de hardware.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

Para ilustrar esses conceitos e sua estruturação dentro do paradigma orientado a objetos, observe o exemplo da imagem **AA**, que traz a abstração do problema base de um veterinário necessitando organizar seu sistema de controle de animais, produtos e serviços.

Como os objetos representam instâncias de classes, uma forma de se definir uma classe é observando o que a abstração pode fornecer de informações sobre o problema real, de forma que se possa pensar em como seria a estrutura de um objeto instanciado com atributos relevantes e como seriam os dados contidos nestes atributos.

Como cada instância de classe representa um conjunto particular de características agrupadas em cada objeto gerado a partir da classe, imaginar o que poderia ser estruturado em forma de objeto, pode ser uma boa opção para se iniciar a definição de classes.

Os animais, por exemplo, podem ser imaginados como classes, pois objetos instanciados a partir desta classe poderiam estar associados a cada animal atendido pelo veterinário com seus atributos específicos como raça, cor, nome, idade, peso, e identificação do dono.

Já os atributos relativos aos donos não precisam ser incluídos diretamente na mesma classe dos animais, pois os atributos dos animais e seus donos não são os mesmos e nem possuem muita relação, e assim, convém definir uma classe para instanciar animais e outra classe para instanciar pessoas.

Assim, já seria possível a obtenção de duas classes com atributos característicos, e também poderiam ser definidos métodos para que os possíveis dados para objetos instanciados pudessem ser trabalhados de forma adequada.

Alguns métodos são essenciais para a entrada de dados e a obtenção de dados chamados de **set()** e **get()**, nomenclatura padrão para essas funcionalidades, mas podem ser definidos métodos menos convencionais para especificidades do problema a ser resolvido.

Os métodos necessitam de comunicação entre si muitas vezes, pois um método pode acionar outro, e a mecânica de execução de métodos é baseada em uso da memória de forma dinâmica de forma que um método ocupa a memória ao ser acionada como todas as estruturas de dados necessárias para sua execução.

Depois, caso outro método seja executado a partir de uma chamada do método em execução, o status do método chamador é pausado e uma nova alocação de memória é feita para os recursos necessários para o novo método.

Ao final da execução do método chamado, dados podem ser passados como retorno para o método chamador e a memória utilizada pelo segundo método é liberada para uso pelo sistema operacional e os dados ali contidos são considerados descartados.

O método chamador volta a atividade, e continua seu processamento, sendo que ao fim de sua execução, seus recursos de memória também são liberados ao sistema operacional, e assim se repetirá o processo para outros métodos executados posteriormente durante a execução do software em si.

Os conceitos ligados à orientação a objetos são variados, e cada linguagem de programação implementa um determinado conjunto de conceitos e os adapta às suas necessidades, supondo o uso de cada mecanismo aplicado a determinados problemas que poderão ser resolvidos com estes recursos. Assim, linguagens que se propõem a resolver problemas mais variados podem necessitar de mais conceitos, e estes implementados com maior possibilidade de variação para uma maior gama de problemas.

Acesse o link:[Disponível aqui](https://www.guj.com.br/t/definicoes-sobre-orientacao-a-objetos/321141)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Abstração
- Conceitos de Classe, Atributo, Método e Objeto

Para complementar seus estudos, assista à videoaula a seguir: