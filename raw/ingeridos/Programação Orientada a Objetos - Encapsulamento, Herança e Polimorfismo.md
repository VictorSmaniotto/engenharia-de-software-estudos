---
title: "Aula 07 - Programação Orientada a Objetos - Encapsulamento, Herança e Polimorfismo"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-07.html"
author:
published:
created: 2026-05-11
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 07 - Programação Orientada a Objetos - Encapsulamento, Herança e Polimorfismo

A orientação a objetos é um paradigma mais moderno que a programação imperativa ou estruturada, e por isto pode ser implementada de forma a conter conceitos mais evoluídos computacionalmente, sendo próxima das necessidades de desenvolvimento de software dos dias atuais de certa forma.

Isso em função também da forma como se desenvolve softwares atualmente, permitindo uma maior independência entre os componentes de um software ou sistema computacional composto de módulos e que funcione na web, por exemplo.

Algumas características são essenciais no paradigma orientado a objetos como a definição da estrutura dos códigos em função de classes com seus atributos e métodos para que objetos sejam instanciados para o armazenamento e processamento de dados.

Outros aspectos não são obrigatórios, mas são o diferencial deste paradigma em relação aos outros e devem ser conhecidos e explorados de forma que possam ser aplicados na implementação de códigos e o real paradigma orientado a objetos possa ser aplicado no desenvolvimento de software.

Linguagens como C e Pascal não suportam a orientação a objetos, mas variações da linguagem C como C++, C# e Objective-C suportam o desenvolvimento orientado a objetos sendo opcional seu uso ou obrigatório dependendo da linguagem derivada de C.

Outras linguagens como Python, PHP e JavaScript permitem que seus códigos possam conter aspectos do paradigma orientado a objetos ou tenham seus códigos escritos de forma estruturada, por exemplo, ficando a escolha por conta de especificidades da solução computacional ou conhecimentos do codificador.

Linguagens como Java e Objective-C trabalham com conceitos de orientação a objetos nativamente e necessitam que seus códigos sejam implementados baseados em classes, sem a possibilidade de programação puramente estruturada, por exemplo.

## Encapsulamento

Um conceito muito importante da orientação a objetos é o chamado **encapsulamento,** que contribui para que as estruturas de classes sejam transparentes para outras classes e todo o conteúdo de uma classe seja empacotado e independente de meios externos à classe.

A ideia de encapsular componentes de uma classe permite maior segurança aos dados que são mantidos pela classe e os processos aos quais são submetidos, tornando também o software mais confiável, pois os dados são processados de forma mais adequada e tendo assim comportamentos menos inesperados.

O que define a base do encapsulamento são palavras reservadas contidas nas linguagens de programação que aceitam este paradigma, servindo para definir o nível de visibilidade de classes, atributos e métodos dentro de um software.

Em geral, as linguagens de programação utilizam três níveis de encapsulamento utilizando as mesmas palavras reservadas *public, private e protected* para diferenciar estes níveis e definir o grau de transparência do código.

Geralmente o chamado modificador de acesso *private* é utilizado em elementos que não devem ser exibidos fora da estrutura na qual foi declarado, pois a ideia deste modificador é deixar qualquer atributo ou método de uma classe totalmente inacessível por outras classes e assim, controlar o que ocorre com estes componentes de forma mais segura.

Na declaração de um atributo ou método é comum que a sintaxe exija que um tipo de dado seja indicado, depois o nome do atributo ou método, e por fim, parâmetros que possam ser associados aos métodos são indicados entre parênteses.

O modificador de acesso *private* é posto logo no início desta sintaxe, antes do tipo de dado associado, aumentando e complementando a sintaxe de declaração de atributos e métodos.

Classes não são normalmente definidas como privadas, pois elas são a única forma de acesso a toda a estrutura de atributos e métodos internos a ela, e se não for permitido acesso a ela, a classe toda ficaria em um nível de encapsulamento inacessível e inutilizável.

Outro tipo de modificador de acesso é público, utilizando a palavra reservada *public* que atua de forma inversa a *private*, permitindo a visibilidade de classes, atributos ou métodos dentro das limitações definidas conceitualmente por ada linguagem.

As classes são sempre do tipo *public*, pois como dito anteriormente, são o meio de acesso a todos os atributos e métodos contidos nela, sendo então necessário que esta seja visível e possa ser chamada por quaisquer outras classes pertencentes ao mesmo software que também pode ser definido por pacote, por exemplo, dependendo da linguagem de programação.

Para que se possa ter um nível adequado de encapsulamento, o uso do modificador *public* em atributos e métodos não é ideal, pois dá certo nível de liberdade de acesso que pode ser indesejável do ponto de vista de segurança e transparência no código, sendo mais comum o uso deste nível de acesso mais em classes.

Outro modificador de acesso comum em linguagens de programação é dito protegido, utilizando a palavra reservada *protected* para que atributos e métodos de uma classe possam ser acessados por classes ligadas à classe ao qual pertencem por um mecanismo da orientação a objetos chamado de **herança**, que será discutido logo adiante.

Neste nível de visibilidade, classes que sejam ligadas entre si podem compartilhar atributos ou métodos protegidos de forma que esta permissão ocorra apenas do sentido de uma das classes para a outra, sendo a classe que contém os atributos ou métodos protegidos é chamada de classe pai (mãe) ou superclasse dependendo dos autores, e a classe ou as classes que estejam interligadas à superclasse e possam ter acesso aos elementos protegidos são ditas **classes filhas ou subclasses**.

## Herança

Partindo da ideia do encapsulamento, foi visto que existem diferentes níveis de visibilidade associados aos termos *public*, *private* e *protected*, sendo que este último depende do conceito a ser tratado a partir deste ponto.

A herança é outra característica muito importante do paradigma orientado a objetos, pois permite que classes ligadas possam possuir um nível de acesso diferenciado em atributos e métodos contidos nestas.

Algumas características são importantes, pois afetam diretamente a possibilidade de uso deste recurso, sendo que existem limitações que devem ser observadas no projeto de software que se baseie neste paradigma e necessite então de uma estruturação de classes de forma que não sejam confundidos os modificadores de acesso utilizados e as regras de herança entre classes respeitadas.

Uma classe pode herdar atributos e métodos de outra classe, sendo a classe que herda chamada de subclasse, podendo pela herança ter acesso a dados de atributos da superclasse, podendo modifica-los, ou usar métodos da superclasse para reduzir redundância de código.

Para ilustrar a herança, podemos imaginar classes genéricas representando veículos, animais ou produtos, sendo estas consideradas superclasses com atributos gerais como fabricante, raça ou data de fabricação respectivamente, e métodos para manipulação destes atributos como os métodos get() e set() que são os mais comuns em classes.

Classes como utilitários ou passeio podem representar outras classes mais específicas de veículos, assim como peixes e mamíferos podem representar classes mais específicas de animais, e possuem os mesmos atributos das classes veículos e animais, mas necessitam de mais atributos específicos e métodos get() e set() diferenciados.

Partindo destas classes, pode-se considerar, por exemplo, veículos como sendo uma superclasse e utilitários e passeio, duas subclasses de veículos, assim como animais pode representar uma superclasse, e peixes e mamíferos, subclasses desta superclasse.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a07-figura1.svg)

Fonte: O autor.

A imagem traz um exemplo de classes e superclasses ilustrando a classe Atividade como sendo uma superclasse mais geral e ligada a esta classe, outras três mais específicas de Indústria, Comércio e Serviços.

Estas três subclasses não são totalmente dependentes da superclasse, mas podem se beneficiar do que ela oferece para complementação e redução de código por evitar repetição desnecessária, além de estruturar de forma mais coerente a modelagem do software em si.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a07-figura2.svg)

Fonte: O autor.

Em complemento à imagem anterior, a imagem acima traz agora o restante dos principais componentes das classes, sendo importante observar que as subclasses possuem especificidades também em seus atributos e métodos, utilizando os atributos e métodos da superclasse quando necessário através da herança.

A herança, assim como todos os conceitos de orientação a objetos deve ser compreendido de forma adequada, pois a programação neste paradigma pode ser simples se não forem utilizados muitos mecanismos próprios do paradigma, tornando um código similar à programação imperativa, mas se os conceitos importantes como herança e polimorfismo forem utilizados, respeitando as limitações impostas pelo encapsulamento definido em um código, o resultado final tende a se distanciar de códigos escritos em linguagens imperativas.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

## Polimorfismo

Outra característica importante da orientação a objetos é chamada de polimorfismo que complementa a herança, proporcionando que subclasses possam personalizar ainda mais suas funcionalidades em relação ao que existe na superclasse a qual esteja associada.

A ideia se baseia na suposição de que uma superclasse possua um método que atenda aos seus requisitos, e subclasses associadas a esta superclasse utilizem este mesmo método, mas tenham alguma variação nos requisitos para este método, e partindo dessa necessidade, o polimorfismo permite que uma subclasse reescreva métodos de uma superclasse usando o mesmo nome e assim, podendo personalizar este método para seu uso.

Tomando como exemplo a superclasse “Animais” e duas subclasses “Mamíferos” e “Peixes”, um método de locomoção poderia existir em Animais, pois todos os animais dentro do escopo do software teriam a capacidade de se mover, mas no caso dos mamíferos, existem propriedades de locomoção diferenciadas em relação ao que ocorre na classe Peixes como o fato de mamíferos poderem andar e nadar, mas os peixes apenas nadarem, excetuando particularidades que possam ocorrer.

Dessa forma, o uso do polimorfismo se mostra como um excelente mecanismo para que classes possam estar interligadas sem prejudicar as particularidades existentes, mantendo as características de cada uma, sem a necessidade de adaptações quando ocorre a ligação por herança normalmente.

Aprender os conceitos de orientação a objetos é bastante importante para compreender códigos, e muitas vezes é preciso exemplos em alguma linguagem para que se possa compreender os conceitos. Neste site, os conceitos são avaliados sobre exemplos que podem auxiliar a compreensão destes, mas é preciso conhecer a base da linguagem para que se possa interpretar corretamente cada conceito dentro do restante do código.

Acesse o link:[Disponível aqui](http://www.linhadecodigo.com.br/artigo/307/introducao-a-orientacao-a-objetos.aspx)

![início do conecte-se](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-conecte-se-center.svg)

Fonte: Freepik.

![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/a04-img07.jpg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Encapsulamento
- Herança
- Polimorfismo

Para complementar seus estudos, assista à videoaula a seguir: