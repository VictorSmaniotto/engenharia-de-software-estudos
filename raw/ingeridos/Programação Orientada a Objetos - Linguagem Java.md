---
title: "Aula 08 - Programação Orientada a Objetos - Linguagem Java"
source: "https://ead.unimar.br/aulas/linguagens-de-programacao/aula-08.html"
author:
published:
created: 2026-05-11
description:
tags:
---
Disciplina: Linguagens de Programação
Aula 08 - Programação Orientada a Objetos - Linguagem Java

Provavelmente, a linguagem mais popular para uso da orientação a objetos seja Java, e é a linguagem ideal para aplicar os conceitos deste paradigma com exemplos demonstrativos de aspectos ligados aos conceitos definidos na parte conceitual da orientação a objetos.

## Linguagem Java

Em Java os tipos básicos de dados não variam muito da linguagem C estruturada, por exemplo, pois os dados puros em si se mantêm como números inteiros, decimais de ponto flutuante, caractere e lógico, mas as estruturas de dados sofrem muita variação em função de simplificações da linguagem em relação à C para que seja uma linguagem de mais alto nível.

Os tipos de dados em Java são pensados para que estruturas mais complexas em termos de implementação e uso sejam simplificadas em sua implementação básica, e assim, listas são mais facilmente manipuladas por tipos mais genéricos que na linguagem C, por exemplo, onde estruturas de dados como listas podem ser mais complexas em sua implementação e uso.

Existe o tipo de dado coleção, definido como *ArrayList* em Java, por exemplo, que serve para que objetos instanciados de classes sejam armazenados em forma de vetor, não podendo ser utilizado para tipos primitivos como inteiros ou caracteres, por exemplo, e para que um dado primitivo possa ser adicionado em uma *ArrayList*, é preciso que seja inserido em um objeto antes.

A medida que a linguagem evoluiu, a forma como os dados primitivos e tipos mais complexos foi sendo melhorada e a inserção de dados primitivos em um *ArrayList* foi sendo melhorada, assim como outras funcionalidades e novas implementações para tornar a linguagem Java sempre atual e com uma variedade maior de recursos a cada nova versão.

Também existem as diferenças em função da mudança de paradigma que obrigam que a estruturação de todo o código seja diferente pela inserção da ideia de classes ao invés de registros, por exemplo.

O exemplo da imagem a seguir traz a base de um código em linguagem Java para análise de sua estrutura, tipos básicos de dados e estruturação de classes com seus atributos e métodos.

**package Exemplos;**

**import java.util.Scanner;**

**class Main {**

**public static void main(String\[\] args) {**

**int resposta;**

**ValidaIdade obj;**

**obj = new ValidaIdade();**

**resposta = obj.setIdade();**

**if (resposta == 1)**

**System.out.printf("Maior de Idade");**

**else**

**System.out.printf("Menor de Idade");**

**}**

**}**

**class ValidaIdade {**

**private int idade;**

**public ValidaIdade () {**

**idade = 0;**

**}**

**public int setIdade() {**

**Scanner dado = new Scanner(System.in);**

**System.out.printf("Informe a idade: ");**

**idade = dado.nextInt();**

**dado.close();**

**if (idade >= 18)**

**return 1;**

**else**

**return 0;**

**}**

**}**

Fonte: autor.

Observando o exemplo, temos um código simples, mas completo que ilustra alguns fundamentos da linguagem Java dentro do paradigma orientado a objetos como a definição das classes **Main** e **ValidaIdade**.

Estas duas classes servem de exemplo da estrutura semântica e sintática da linguagem, mas também apresenta a definição de um atributo idade que utiliza o modificador de acesso *private* para mantê-lo encapsulado à sua classe de origem e para que possa ser utilizado, é necessário que um objeto *obj* seja instanciado a partir da classe ValidaIdade.

O método de instanciação de objetos em Java e a compreensão da semântica e sintaxe envolvidas no processo não é algo trivial, pois os conceitos de orientação a objetos não são tão simples como os da programação estruturada em alguns aspectos, mas a simplificação do uso de estruturas de dados na linguagem Java, por exemplo, servem como compensação.

A partir do momento em que um objeto está instanciado, os métodos a serem acessados devem conter antes de seu nome, a indicação do objeto ao qual estará associado para que o processamento de dados realizado se refira aos dados contidos nos atributos deste objeto.

Para analisar o código como um todo, é importante observar a sua sequência de execução, iniciando pela classe que possui o método main() que é padrão da linguagem como ponto de partida, sendo uma exceção da própria implementação da linguagem que não precisa ser associado a um objeto instanciado, pois isto não seria possível logo na inicialização da aplicação, pois os objetos vão sendo instanciados ao longo da execução da aplicação quando necessário.

Depois de iniciada a execução do método main(), uma variável resposta é declarada, e neste momento é importante observar que não se trata de um atributo de classe, pois se encontra declarada dentro de um método, e os atributos são declarados fora dos métodos, sendo algo comum da semântica da linguagem Java, mas que pode confundir a leitura de códigos inicialmente.

Logo em seguida, pelo fluxo de execução do software, um objeto é instanciado para a classe ValidaIdade, para que seus atributos e métodos possam ser utilizados para a realização de processos necessários, como o recebimento do dado para o atributo idade, sendo que um método set() e outro get() poderiam ser implementados apenas para gerenciamento deste atributo, mas foi optado pela criação de um método que recebe e já valida a idade para retornar um resultado já processável pelo restante do software.

Este retorno é então verificado em uma estrutura de decisão que verifica entre 0 e 1 os valores possíveis de retorno do método, sendo este retorno chamado de mensagem que é passada entre métodos durante o fluxo de execução.

Por fim, o código avalia o valor recebido na variável de apoio resposta declarada para uso pelo método main() e dependendo de cada possível resposta, mensagens são exibidas ao usuário, de maneira informativa apenas.

Alguns pontos relevantes podem ser comentados como a classe System, padrão da linguagem e que pode ser diretamente acessada sem a necessidade de importação como foi feito com a classe java.util.Scanner para que se possa receber dados pelo objeto instanciado com base nesta classe importada.

Por fim, outro ponto importante deste exemplo da imagem 21 é o uso de um construtor *public* ValidaIdade() para inicializar o atributo idade com zero, de forma a garantir que não exista um valor inadequado contido na área de memória alocada para o atributo.

Um último aspecto importante é que em Java, assim como em outras linguagens de programação, o encapsulamento pode permitir a inclusão de mais de uma classe sob um mesmo software através do uso do conceito de encapsulamento de nomeação segundo (SEBESTA, 2011), onde o uso da palavra reservada *package* permite que várias classes possam estar associadas a um mesmo pacote e façam parte de um conjunto de códigos Java que compõem a aplicação completa.

Partindo da ideia do pacote, na linguagem Java não é muito aconselhável que se tenha mais de uma classe num mesmo arquivo, mas caso sejam interligadas e uma classe seja dominante e relacionada à outra classe dependente, é possível então declarar a classe dominante como pública e a outra ser mantida ser modificador de acesso (sendo então default) ou *private*, pois se for colocada como *public* também, cria-se uma confusão na semântica de código em relação à definição da linguagem.

**public class Profissao {**

**protected void trabalhar () {**

**System.out.println( "Profissional trabalha em sua função." );**

**}**

**}**

**public class Agricultor extends Profissao {**

**private void trabalhar () {**

**System.out.println( "Agricultor planta." );**

**}**

**}**

**public class Pedreiro extends Profissao {**

**private void trabalhar () {**

**System.out.println( "Pedreiro constrói." );**

**}**

**}**

Fonte: autor.

No exemplo de classes da imagem, temos três classes que, pelos seus nomes, indicam que pode existir uma relação entre elas, e isto pode ser claramente observado através do uso da palavra reservada *extends* em duas das classes.

A palavra *extends* indica ao compilador que as classes “Agricultor” e “Pedreiro” são classes que funcionam como extensões da classe Profissao, e assim, as duas classes que utilizam a palavra *extends* se tornam subclasses da classe indicada após a palavra reservada, ou neste caso, Profissao que se torna uma superclasse de onde as subclasses podem ter acesso a atributos e métodos protegidos através da herança.

Isso significa que as subclasses “Agricultor” e “Pedreiro” podem acessar atributos e métodos da superclasse Profissao, mas um ponto que deve ser levado em consideração para uso da herança em Java é o encapsulamento, pois ele determina o que pode ser visto em até três níveis.

O primeiro privado utilizando a palavra reservada *private* para identificar um atributo ou método como específico da classe e invisível às demais classes de um pacote de classes que compõem uma aplicação.

O segundo é público que utiliza a palavra reservada *public* que permite que atributos ou métodos sejam sempre visíveis por outras classes de um mesmo pacote, reduzindo muito a aplicação do encapsulamento e com isto deixando toda a aplicação mais exposta.

E terceiro a visibilidade privada que utiliza a palavra reservada *protected* que permite que subclasses acessem atributos ou métodos de uma superclasse, sendo esta, a visibilidade adequada para se manter as propriedades de encapsulamento e herança adequadas a um pacote de classes de uma aplicação completa.

Outro conceito extremamente importante no exemplo da imagem acima e tda imagem a seguir, é o de polimorfismo, em que o método trabalhar() é reescrito nas subclasses para adequar seus processos às especificidades destas subclasses em relação ao que ocorre no método de mesmo nome na superclasse.

A ideia deste conceito complementar ao da herança é de que uma subclasse possui particularidades em relação a uma superclasse, e assim, pode ser necessário adaptar o processamento de dados que ocorrem na subclasse em relação ao que ocorre em um mesmo método da superclasse.

Com este exemplo então, é possível observar a ocorrência de três dos principais conceitos do paradigma de orientação a objetos:

- Encapsulamento com o uso das palavras reservadas *private*, *public* e *protected* para controlar a visualização de atributos, métodos e classes.
- Herança com o uso da palavra extends para indicar quando uma classe representa uma subclasse de outra classe que se torna superclasse e pode permitir que uma subclasse tenha acesso a atributos e métodos através de instâncias das subclasses.
- Polimorfismo para que métodos de uma subclasse equivalentes a de sua superclasse possam ser reescritos para se adaptarem aos requisitos da subclasse.

A programação orientada a objetos em linguagem Java possui muitos recursos próprios e merece atenção especial por parte dos interessados em aprender uma linguagem de programação orientada a objetos, pois uma linguagem ainda dominante no mercado e possui uma vasta coleção de bibliotecas implementadas e testadas, e frameworks desenvolvidos a partir da linguagem.

Outra possibilidade mostrada na imagem 23 é o uso de classes e métodos abstratos que podem ser utilizados em classes que apenas servem como estrutura para subclasses que irão implementar o conteúdo destas classes realmente, tendo assim, instruções dentro do métodos das subclasses, ao contrário dos métodos de classes abstratas que não contém instruções, apenas a declaração de métodos para referência estrutural das classes da aplicação.

**public abstract class Profissao {**

**public abstract void trabalhar ();**

**}**

**public class Agricultor extends Profissao {**

**private void trabalhar () {**

**System.out.println( "Agricultor planta." );**

**}**

**}**

**public class Pedreiro extends Profissao {**

**private void trabalhar () {**

**System.out.println( "Pedreiro constrói." );**

**}**

**}**

Fonte: autor.

Outros conceitos relacionados à orientação a objetos e presentes na linguagem Java como o uso de interfaces que servem como classe padrão para a implementação de outras classes, tendo apenas declarações de métodos sem implementá-los, pois serão implementados nas classes indicadas pela palavra reservada *implements*.

**public interface Profissao {**

**public void trabalhar ();**

**}**

**public class Agricultor implements Profissao {**

**@Override**

**private void trabalhar () {**

**System.out.println( "Agricultor planta." );**

**}**

**}**

**public class Pedreiro implements Profissao {**

**@Override**

**private void trabalhar () {**

**System.out.println( "Pedreiro constrói." );**

**}**

**}**

Fonte: autor.

Observando o exemplo de código da imagem acima é possível que se faça uma comparação com o exemplo da figura anterior, e imagine que são duas formas diferentes de se fazer exatamente a mesma coisa, mas não são métodos diferentes para atingir o mesmo objetivo.

Um ponto de atenção no exemplo é que se usa a palavra reservada @Override que possui a função de informar ao compilador que o método sendo implementado a seguir é uma modificação de outro de igual nome em uma superclasse, e caso este nome não seja encontrado na superclasse, um erro de compilação ocorrerá, auxiliando na manutenção de código, pois nomes de classes, atributos e métodos podem ser modificados, mesmo não sendo recomendado em códigos maiores.

As interfaces são tipos de classes abstratas que permitem de forma improvisada um recurso chamado de herança múltipla que significa que uma classe pode ser baseada em mais de uma classe para ser estruturada e posteriormente instanciar objetos.

A partir da versão 8 de Java, a herança múltipla foi implementada e pode ser normalmente utilizada seguindo uma sintaxe semelhante à do exemplo da imagem a seguir em que a indicação da herança múltipla ocorre na declaração da subclasse definida a partir de duas outras superclasses separadas por vírgulas.

**public interface Profissao {**

**default void trabalhar ();**

**System.out.println( "Profissional trabalha em sua função." );**

**}**

**public interface Contrato {**

**default void regime ();**

**System.out.println( "Profissional contratado CLT." );**

**}**

**public class Emprego implements Profissao, Contrato {**

**}**

**public class Cadastro {**

**public static void main (String\[\] args) {**

**Emprego emprego = new Emprego();**

**emprego.trabalhar();**

**emprego.regime();**

**}**

**}**

Fonte: autor.

Com estes conceitos, foi possível observar como uma linguagem de programação implementada com base no paradigma orientado a objetos é estruturada, lembrando que é apenas uma amostra da linguagem e de alguns de seus conceitos, sendo que para conhecer mesmo a linguagem, é preciso buscar mais fontes de pesquisa e praticar muito a leitura, interpretação e criação de códigos.

Existem conceitos da orientação a objetos que não são utilizados, a menos que o desenvolvedor tenha uma demanda específica em relação ao uso destes recursos ou imagine sua solução com base nestes conceitos. É o caso do uso de classes abstratas que servem de modelo para outras classes não sendo instanciadas para a geração de objetos, ou as interfaces que representam tipos especiais de classes abstratas que utilizam atributos mais específicos (*static* e *final*) tendo apenas métodos abstratos e públicos, sem terem o seu código para processamento de dados, apenas as estruturas das classes e componentes destas. Esse mecanismo de criação de interfaces permite que algumas situações sejam solucionadas como no caso hipotético onde classes A, B e C sejam herdeiras da classe abstrata Z. E queiramos atribuir apenas as classes B e C determinado comportamento. Se fosse feito pela classe abstrata Z todos herdariam, então resolvemos isso criando uma interface e a relacionamos apenas com B e C.

![início do para gabaritar](https://ead.unimar.br/aulas/linguagens-de-programacao/images/cx-gabaritar-center.svg) <video controls=""><source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/linguagens-de-programacao/videos/bg-video_1-transcode.webm"></video> ![](https://ead.unimar.br/aulas/linguagens-de-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Linguagem Java

Para complementar seus estudos, assista à videoaula a seguir: