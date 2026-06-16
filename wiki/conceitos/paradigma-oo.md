---
titulo: Paradigma Orientado a Objetos (OO)
tipo: conceito
tags: [paradigma, orientacao-a-objetos, OOP, classes, heranca, polimorfismo, encapsulamento]
disciplina: Linguagens de Programação
fontes: [lp-m2-a01-paradigmas-de-programacao, lp-a06-poo-conceitos, lp-a07-poo-encapsulamento-heranca-polimorfismo, lp-a08-poo-linguagem-java]
criado: 2026-05-07
atualizado: 2026-05-11
---

# Paradigma Orientado a Objetos (OO)

## Definição

Derivação do [paradigma imperativo](paradigma-imperativo.md), segundo Sebesta (2011). Estrutura o programa em **classes** que agrupam dados (atributos) e comportamentos (métodos), das quais **objetos** são instanciados. Permite maior independência entre componentes e maior reutilização de código em relação ao estruturado.

> "A programação orientada a objetos possui foco na abstração de dados estruturando-os como atributos de classes que são evoluções das funções em programação imperativa e permitem uma maior independência entre estes componentes que acabam sendo mais facilmente reutilizados em novos softwares." (LP A2)

Citado como paradigma "favorito do mercado atualmente" (LP A6). A linguagem **Smalltalk** (1980s) é uma das primeiras a usar OO como base.

## Evolução em relação ao Estruturado

| Aspecto | Estruturado | OO |
|---------|------------|-----|
| Organização de dados | Registros (`struct`) separados das funções | Classes integram dados (atributos) e comportamentos (métodos) |
| Reúso | Sub-rotinas reutilizáveis | Classes e hierarquias de herança reutilizáveis |
| Abstração | Funcional | Modelagem de entidades do mundo real |

## Os Quatro Elementos Centrais

Ver [POO: Classes, Atributos, Métodos e Objetos](poo-classes-atributos-metodos.md) para detalhes.

- **Classe**: modelo/template que define atributos e métodos
- **Atributo**: propriedade da classe; armazena dados do objeto
- **Método**: sub-rotina da classe; processa atributos
- **Objeto**: instância particular da classe com dados próprios

## Os Três Pilares Diferenciais

| Pilar | Definição resumida | Página |
|-------|--------------------|--------|
| [Encapsulamento](encapsulamento.md) | Controle de visibilidade via `private`/`public`/`protected` | [→](encapsulamento.md) |
| [Herança](heranca.md) | Subclasse herda atributos e métodos de superclasse | [→](heranca.md) |
| [Polimorfismo](polimorfismo.md) | Subclasse reescreve método da superclasse (`@Override`) | [→](polimorfismo.md) |

## Linguagens e Grau de Suporte

| Linguagem | Suporte a OO |
|-----------|-------------|
| C, Pascal | Nenhum |
| C++, C#, Python, PHP, JavaScript | OO opcional (coexiste com estruturado) |
| Java, Objective-C | OO obrigatório (tudo em classes) |

## Linguagem Canônica

A [Linguagem Java](linguagem-java.md) é a referência principal para estudo do OO: OO nativo, bytecode portável (JVM), e rica coleção de bibliotecas e frameworks.

## Relações

- [Paradigma Estruturado](paradigma-estruturado.md) — base a partir da qual o OO evoluiu
- [Classes Abstratas e Interfaces](classes-abstratas-interfaces.md) — mecanismos avançados de OO
- [Linguagem Java](linguagem-java.md) — linguagem canônica do OO
- [Programação Funcional](paradigma-funcional.md)

## Fontes

- [LP M2 A1 — Paradigmas de Programação](../fontes/lp-m2-a01-paradigmas-de-programacao.md)
- [LP A2 — Classificação de Paradigmas](../fontes/lp-a02-classificacao-de-paradigmas.md)
- [LP A6 — POO: Conceitos de Classes, Atributos, Métodos e Objetos](../fontes/lp-a06-poo-conceitos.md)
- [LP A7 — POO: Encapsulamento, Herança e Polimorfismo](../fontes/lp-a07-poo-encapsulamento-heranca-polimorfismo.md)
- [LP A8 — POO: Linguagem Java](../fontes/lp-a08-poo-linguagem-java.md)
