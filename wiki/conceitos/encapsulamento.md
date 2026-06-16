---
titulo: Encapsulamento
tipo: conceito
tags: [poo, encapsulamento, modificadores-de-acesso, private, public, protected]
disciplina: Linguagens de Programação
fontes: [lp-a07-poo-encapsulamento-heranca-polimorfismo, lp-a08-poo-linguagem-java]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Encapsulamento

## Definição

Pilar do paradigma OO que consiste em **empacotar atributos e métodos dentro de uma classe**, tornando-a independente e controlando o que é visível externamente. Contribui para segurança dos dados e confiabilidade do software ao garantir que dados sejam processados apenas pelos mecanismos definidos pela própria classe.

## Modificadores de Acesso

Palavras reservadas que definem o nível de visibilidade de classes, atributos e métodos:

| Modificador | Visibilidade | Uso típico |
|-------------|-------------|------------|
| `private` | Apenas dentro da própria classe | Atributos (padrão recomendado) |
| `public` | Qualquer classe do pacote/software | Classes; métodos de acesso externo |
| `protected` | Classe própria + subclasses via herança | Atributos/métodos que subclasses precisam acessar |

## Regras Práticas

- **Classes** são sempre `public` — são o único ponto de acesso a seus atributos e métodos
- **Atributos** devem ser preferencialmente `private` — acesso controlado por métodos `get()`/`set()`
- **Usar `public` em atributos** reduz o encapsulamento e aumenta a exposição e fragilidade do software
- **`protected`** é o modificador adequado quando há hierarquia de herança e subclasses precisam acessar elementos da superclasse

## Encapsulamento de Nomeação (Sebesta, 2011)

Além do encapsulamento de dados, existe o encapsulamento de **nomeação**: agrupamento de classes relacionadas em um mesmo **pacote** (`package` em Java), organizando o software em módulos coesos.

## Relações

- [Herança](heranca.md) — `protected` só faz sentido no contexto da herança
- [POO: Classes, Atributos, Métodos e Objetos](poo-classes-atributos-metodos.md) — atributos são encapsulados por padrão
- [Linguagem Java](linguagem-java.md) — implementação concreta com `private`, `public`, `protected`, `package`
- [Critérios de Avaliação de Linguagens](criterios-avaliacao-linguagens.md) — encapsulamento contribui para confiabilidade (Sebesta)

## Fontes

- [LP A7 — POO: Encapsulamento, Herança e Polimorfismo](../fontes/lp-a07-poo-encapsulamento-heranca-polimorfismo.md)
- [LP A8 — POO: Linguagem Java](../fontes/lp-a08-poo-linguagem-java.md)
- [Sebesta (2011)](../autores/sebesta.md)
