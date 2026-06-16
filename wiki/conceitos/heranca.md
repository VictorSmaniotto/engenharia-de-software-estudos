---
titulo: Herança
tipo: conceito
tags: [poo, heranca, superclasse, subclasse, extends, reutilizacao]
disciplina: Linguagens de Programação
fontes: [lp-a07-poo-encapsulamento-heranca-polimorfismo, lp-a08-poo-linguagem-java]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Herança

## Definição

Mecanismo do paradigma OO que permite que uma **subclasse** herde atributos e métodos de uma **superclasse**, reduzindo redundância de código e permitindo extensão de funcionalidades sem reescrita.

> Uma subclasse pode acessar dados de atributos da superclasse, modificá-los, ou usar métodos da superclasse para reduzir redundância de código. (LP A7)

## Terminologia

| Termo | Sinônimo | Papel |
|-------|----------|-------|
| **Superclasse** | Classe pai / classe mãe | Define atributos e métodos gerais |
| **Subclasse** | Classe filha | Estende a superclasse com especificidades |

## Como Funciona

- A superclasse define características comuns (ex: `Veículos` com fabricante, ano)
- Subclasses herdam essas características e adicionam as próprias (ex: `Utilitários` com capacidade de carga)
- Atributos/métodos `protected` na superclasse são acessíveis pelas subclasses
- Atributos/métodos `private` na superclasse **não são acessíveis** pelas subclasses
- Subclasses não são totalmente dependentes — usam herança onde é vantajoso

## Exemplos de Hierarquias Típicas

```
Animais (superclasse)
├── Mamíferos (subclasse)
└── Peixes (subclasse)

Veículos (superclasse)
├── Utilitários (subclasse)
└── Passeio (subclasse)

Atividade (superclasse)
├── Indústria (subclasse)
├── Comércio (subclasse)
└── Serviços (subclasse)
```

## Em Java: `extends`

```java
public class Profissao {
    protected void trabalhar() { ... }
}

public class Agricultor extends Profissao {
    // herda trabalhar() e pode sobrescrevê-lo
}
```

## Herança Múltipla

- Java não suporta herança múltipla via `extends` (uma subclasse, uma superclasse)
- Herança múltipla é obtida via **interfaces** (`implements A, B`) — ver [Classes Abstratas e Interfaces](classes-abstratas-interfaces.md)
- Java 8+: interfaces com métodos `default` permitem comportamento herdado de múltiplas fontes

## Relações

- [Encapsulamento](encapsulamento.md) — `protected` é o modificador que habilita herança com segurança
- [Polimorfismo](polimorfismo.md) — complemento natural da herança; subclasses personalizam métodos herdados
- [Classes Abstratas e Interfaces](classes-abstratas-interfaces.md) — alternativas para estruturar hierarquias
- [Linguagem Java](linguagem-java.md) — herança implementada com `extends`

## Fontes

- [LP A7 — POO: Encapsulamento, Herança e Polimorfismo](../fontes/lp-a07-poo-encapsulamento-heranca-polimorfismo.md)
- [LP A8 — POO: Linguagem Java](../fontes/lp-a08-poo-linguagem-java.md)
