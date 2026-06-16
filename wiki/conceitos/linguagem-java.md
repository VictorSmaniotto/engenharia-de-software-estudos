---
titulo: Linguagem Java
tipo: conceito
tags: [java, poo, bytecode, jvm, package, extends, implements, linguagens]
disciplina: Linguagens de Programação
fontes: [lp-a08-poo-linguagem-java]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Linguagem Java

## Definição

Linguagem de programação **orientada a objetos nativa**: todo código deve estar dentro de classes. Provavelmente a linguagem mais popular para OO; compilada para **bytecode** interpretado pela JVM (alta portabilidade).

## Características

| Característica | Detalhe |
|---------------|---------|
| Paradigma | OO obrigatório (sem programação puramente estruturada) |
| Compilação | Código → bytecode (.class) → JVM |
| Portabilidade | Alta — mesmo bytecode em qualquer plataforma com JVM |
| Case sensitive | Sim |
| Ponto de entrada | `main(String[] args)` — único método sem necessidade de objeto |

## Tipos de Dados

- Primitivos (herdados do C): `int`, `float`, `char`, `boolean`
- Listas de objetos: `ArrayList` — não aceita primitivos diretamente
- Tipos evoluem a cada versão para simplificar manipulação de dados

## Estrutura Básica

```java
package NomePacote;           // agrupa classes do software
import java.util.Scanner;    // importa classe externa

class Main {
    public static void main(String[] args) {
        // ponto de entrada; não precisa de objeto instanciado
    }
}
```

## Instanciação de Objetos

```java
NomeDaClasse obj;                  // declaração
obj = new NomeDaClasse();          // instanciação (chama construtor)
obj.nomeMetodo();                  // acesso a método via objeto
```

- Variáveis dentro de métodos ≠ atributos de classe (atributos são declarados fora dos métodos)

## Os Três Pilares OO em Java

| Conceito | Palavra-chave | Página |
|----------|--------------|--------|
| Encapsulamento | `private`, `public`, `protected` | [Encapsulamento](encapsulamento.md) |
| Herança | `extends` | [Herança](heranca.md) |
| Polimorfismo | `@Override` | [Polimorfismo](polimorfismo.md) |

## Classes Abstratas e Interfaces

- `abstract class`: modelo sem instanciação; métodos `abstract` sem implementação
- `interface`: contrato de métodos; permite herança múltipla (`implements A, B`)
- Ver detalhes em [Classes Abstratas e Interfaces](classes-abstratas-interfaces.md)

## Relações

- [Compilação e Interpretação](compilacao-e-interpretacao.md) — Java usa bytecode/JVM (já documentado em LP A3)
- [Paradigma OO](paradigma-oo.md) — Java é a linguagem canônica do paradigma OO
- [Linguagem C](linguagem-c.md) — Java adotou delimitadores e sintaxe do C; eliminou ponteiros

## Fontes

- [LP A8 — POO: Linguagem Java](../fontes/lp-a08-poo-linguagem-java.md)
