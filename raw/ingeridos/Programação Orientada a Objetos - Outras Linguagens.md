---
title: "Programação Orientada a Objetos - Outras Linguagens"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-09.html"
author:
published:
created: 2026-05-19
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 09 - Programação Orientada a Objetos - Outras Linguagens
O paradigma orientado a objetos é bastante popular na atualidade, e várias linguagens de programação foram criadas já usando como base este paradigma – é o caso da linguagem Java. Mas outras foram adaptadas para permitirem o desenvolvimento de código neste paradigma, como ocorreu com a linguagem C que na implementação C++ adicionou a possibilidade de uso deste paradigma.

## Linguagem Smalltalk

Uma linguagem que contempla os conceitos do paradigma orientado a objetos por ser a linguagem que nasceu juntamente com o paradigma é a linguagem Smalltalk, também responsável pelo conceito de interação com usuários através de janelas, segundo Wangenheim (2002).

Por ser uma linguagem aparentemente com pouca variedade de funcionalidades, representa uma linguagem com boa ortogonalidade, ou seja, possui baixa redundância na geração de código.

Outra característica é que as classes que servem para instanciar objetos também são objetos, pois tudo na linguagem Smalltalk são objetos segundo (Wangenheim, 2002), e para se definir classes existe o conceito de metaclasse, e assim, as classes não precisam ser instanciadas para a geração de objetos.

Assim, nessa linguagem, tanto instâncias de classes quanto objetos são criados por um mecanismo de envio de mensagens através do uso da palavra reservada new, assim como em Java.

As classes em Smalltalk possuem também atributos e métodos, além da linguagem ter implementado os mecanismos de herança simples apenas, e tudo que pertence a uma superclasse é automaticamente herdado por suas subclasses. O polimorfismo também faz parte da implementação da linguagem permitindo que duas classes distintas possuam um mesmo nome em superclasse e subclasse.

Outro ponto relevante dentro da linguagem Smalltalk que se refletiu em Java foi a compilação para geração de arquivo intermediário chamado de *bytecode* e que deve ser interpretado por uma máquina virtual instalada e compatível com o sistema operacional em uso.

Com relação à definição de identificadores, a linguagem Smalltalk, assim como C e Java, é *case* *sensitive*, diferenciando letras minúsculas de maiúsculas, podendo então ser definidas regras de nomenclatura como uso de letras minúsculas para iniciar nomes de atributos e método, e de maiúsculas para nomear classes.

Em relação aos tipos primitivos de dados, a forma como a linguagem trabalha em torno de objetos pode parecer estranha, mas mesmo números simples são considerados objetos instanciados de classes referentes a tipos numéricos, e 10 é considerado um Smallinteger, 23.90 é considerado *float* de ponto flutuante, e um tipo diferente é o fracionário Fraction que será instanciado em frações com divisão não inteira como em 7/3.

A sintaxe da linguagem Smalltalk é um pouco diferente do usual, pois sendo uma das linguagens antigas que serviram de base para outras, foi implementada de forma singular como se pode observar nos exemplos de instruções da imagem:



```Smalltalk
10 timesRepeat: \[Transcript show: ’Smalltalk’\]

1 to: 100 by: 5 do: \[: cont |

Transcript show: (cont printString)

\]

100 to: 200 do: \[: cont |Transcript show: (cont printString)\]

"exemplo de utilização do método whileTrue"

|c|

c:= 0.

\[Transcript show: ('numero', c printString ).

Transcript cr.

c:= c + 1.

c < 10\] whileTrue.

"exemplo de utilização od método whileFalse"

|c|

c:= 0.

\[Transcript show: ('numero', c printString ).

Transcript cr.

c:= c + 1.

c >= 10\] whileFalse.
```

Fonte: Wangenheim (2002).

Nos exemplos de instruções na imagem, nas primeiras três instruções, são definidas estruturas de repetição de três formas semelhantes à maneira como se implementa laços contados em outras linguagens que utilizam a palavra reservada for.

Em Smalltalk, pode optar por utilizar a palavra reservada *timerRepeat* que tem em sua sintaxe diretamente uma determinada quantidade de iterações, e depois, num segundo exemplo, é usada a palavra reservada *to* para indicar delimitadores de início e fim de contagem, e a palavra reservada *by* para informar de quantas em quantas unidades a contagem deve ser realizada.

Depois, ainda no exemplo da imagem acima, as palavras reservadas *whileTrue* (enquanto verdadeiro) e *whileFalse* (enquanto falso) servem para que condições possam ser estabelecidas dentro da sintaxe da linguagem para determinar condições de parada das iterações.

No exemplo contendo *whileTrue*, é declarado um objeto pela instrução |c| que cria uma variável para receber inicialmente o valor 0 para depois ser iniciado um bloco de comandos que primeiramente exibe o valor de c, depois incrementa o valor da variável em uma unidade, executando iterações enquanto o valor de c for menor que 10.

No exemplo utilizando *whileFalse*, o mesmo conjunto de instruções é executado trabalhando sobre o valor de uma variável c, alterando a lógica de controle das iterações enquanto o valor da variável C não for maior ou igual a 10.

Alguns detalhes de sintaxe relevantes são o uso de aspas duplas para comentários e simples para textos a serem exibidos pelo método show(). Também são usados os símbolos de dois pontos para a indicação de parâmetros para comandos e do ponto final como término de comandos. Os colchetes são usados como delimitadores de blocos de comandos e o símbolo | é usado para delimitar identificadores de variáveis.

Assim, percebe-se que conhecendo a base sintática da linguagem, pode-se compreender seus códigos mais facilmente, e a semântica da linguagem não difere muito das demais linguagens, tendo sua estrutura particular de construção de códigos, mas sendo de interpretação até simples em códigos não muito elaborados.

O aprendizado de novas linguagens de programação pode ser mais difícil do que se imagina, pois uma nova linguagem sendo estudada pode ser de um diferente paradigma, fato que por si só já é um dificultador. Pode ocorrer também que a linguagem aceite o mesmo paradigma da linguagem que se domina, mas possa ser multiparadigma e misture conceitos que podem confundir a interpretação de códigos. É importante ler sobre a linguagem e conhecer seus pontos fortes e fracos, saber com base em qual paradigma foi implementada, ver pequenos códigos que sirvam de base para os principais conceitos e estar com a mente aberta para evitar vícios de programação da linguagem já dominada e que possam não ser adequados ou aceitos pela nova linguagem.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg)

## Linguagem C++

Outra linguagem de programação que pode ser utilizada para complementar os estudos neste paradigma é a linguagem C++ que possui as funcionalidades da linguagem C, mas agregando, entre outras funcionalidades e conceitos, o paradigma orientado a objetos.

Complementarmente às estruturas que são adequadas ao uso para armazenamento de dados, as classes com seus atributos e métodos foram implementados, permitindo que a base do paradigma orientado a objetos pudesse ser agregada à programação estruturada, criando assim uma linguagem multiparadigma.

Como na linguagem Java, existem três tipos de modificadores de acesso público, protegido e privado, usando as mesmas palavras reservadas *public*, *protected* e *private* para determinar o grau de encapsulamento de atributos e métodos dentro de uma classe, permitindo assim que além do encapsulamento, herança e polimorfismo tenham espaço para serem implementados como recursos na linguagem.

```c#
#include <iostream>
using namespace std;

class Animal{
	int codigoAnimal;
	int raca;
	string cor;
	string nome;
	string dono;

public:
	void setCodigo (int codigo);
	void setRaca (int raca);
};
```

Fonte: autor.

No exemplo da imagem, um código é implementado, mas se for observado, não há efetivamente código presente, apenas definições de uma classe com seus atributos e métodos, servindo como conteúdo para um arquivo de cabeçalho para o código efetivamente, sendo então estruturado como uma biblioteca que pode ser nomeada “animal.h” ou ‘animal.hpp” (extensão mais específica para a linguagem C++).

O código em si pode ser implementado em outro arquivo chamado “animal.cpp” tendo a extensão padrão da linguagem C++ e a biblioteca criada sendo agregada pelo comando include como é habitual nos códigos da linguagem C e C++ para bibliotecas padrão, e também para aquelas implementadas para a aplicação.

```c#
#include "animal.hpp"
void Animal::setCodigo (int codigo) {
	codigoAnimal = codigo;
}

void Animal::setRaca (int racaAnimal) {
	raca = racaAnimal;
}
```

Fonte: autor.

Neste exemplo da imagem, um arquivo animal.cpp, pode conter a implementação dos métodos indicados nas definições inseridas no arquivo animal.hpp, gerando assim a possibilidade de instância da classe e uso de métodos para ajustar dados de atributos como nas demais linguagens orientadas a objeto.

Um ponto importante é o uso de #include “animal.hpp” para que as definições geradas da classe possam ser acessadas pelo compilador, e assim, sendo feita uma ligação entre o “arquivo.cpp” e o “arquivo.hpp” no momento de se gerar um software executável.

Por fim, o código contido no exemplo da imagem 30 representa o componente principal da aplicação toda, onde a função main() é utilizada, sendo a responsável por iniciar a execução do software, observando que os dois outros arquivos não continham esta função.

Nela, são inseridos os comandos necessários para que a aplicação possa funcionar como esperado, recebendo dados e inserindo-os em atributos de objetos instanciados através dos métodos disponíveis.

```c#
#include "animal.hpp"
void main()
{
Animal pet;
pet.setCodigo (1);
pet.setRaca (3);
}
```

Fonte: autor.

O exemplo da imagem traz a instância do objeto pet utilizando como referência à classe Animal e em seguida, utiliza os métodos set() para atribuir valores aos atributos *codigo* e *raca* do objeto.

Esse terceiro arquivo poderia ter um nome já pensando no software como se chamará e não exatamente como é o nome de uma classe associada, como por exemplo, “petshop.cpp” para que após compilado, o executável final seja chamado por este mesmo nome, simplificando a documentação e compreensão do código todo da aplicação.

Os conceitos de construtores e destrutores também estão presentes, e permitem a garantia de uma correta inicialização de atributos em objetos instanciados através de métodos construtores com o mesmo nome da classe obrigatoriamente. Uma classe também pode ter vários construtores diferentes implementados e só podem ser utilizados através do uso da palavra reservada new ou na instância de um objeto.

O destrutor é chamado quando um objeto não necessita mais ser utilizado devendo ser chamado ao término de seu processamento, usando a interrogação antes do nome de um método de mesmo nome da classe, assim como o construtor.

```c#
class Animal
{
	int codigoAnimal;
	int raca;
	string cor;
	string nome;
	string dono;

	public:
		void Animal (void) {
			codigoAnimal = 0;
			raca = 0;
			cor = “”;
			nome = “”;
			dono = “”;
		}
		
		void ~Animal (void) {
			cout << “Objeto excluído\\n”;

		}
};
```

Fonte: autor.

O exemplo de construtor e destrutor da imagem mostra como se pode implementar este tipo de método, e no construtor são inicializados os valores dos atributos com dados de segurança e no destrutor é exibida uma mensagem informativa da exclusão do objeto.

O encapsulamento pode ser implementado de formas variadas em uma linguagem orientada a objetos, de acordo com as diferentes funcionalidades desejadas como oferta pela linguagem. A linguagem C# é um exemplo de linguagem com modificadores de acesso um pouco diferentes das linguagens C++ e Java, tendo além dos modificadores público, protegido e privado, os modificadores interno, interno protegido, e protegido particular.

Fonte:[Disponível aqui](https://docs.microsoft.com/pt-br/dotnet/csharp/programming-guide/classes-and-structs/access-modifiers)

### Nesta aula estudamos:

- Linguagem Smalltalk
- Linguagem C++

