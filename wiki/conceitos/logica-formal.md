---
titulo: Lógica Formal
tipo: conceito
tags: [logica-formal, proposicoes, operadores-logicos, tabela-verdade, matematica]
disciplina: Linguagens de Programação
fontes: [lp-a13-programacao-logica-conceitos]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Lógica Formal

## Definição

Ramo da matemática que fundamenta o [Paradigma Lógico](paradigma-logico.md). Seu conceito central são as **proposições**: sentenças lógicas que resultam **verdadeiras (V)** ou **falsas (F)**, construídas a partir de relacionamentos entre elementos (Sebesta, 2011 — LP A13).

## Elementos

- **Constante** — símbolo que representa um objeto.
- **Variável** — símbolo que representa objetos diferentes em momentos diferentes; mais próxima da variável matemática do que da variável de uma linguagem imperativa.
- **Termos** simples ou compostos.

## Proposições

- **Simples**: uma única avaliação V/F.
- **Composta**: combina proposições simples por meio de **operadores lógicos**.

## Operadores lógicos

Na lógica: negação, conjunção, disjunção, equivalência, implicação. Na programação, nem todos têm o mesmo uso/símbolo. Expressões matemáticas de conjuntos como "a ⊃ b" (implicação) e "a ∩ b" correspondem às operações **E** e **OU**.

### Tabelas-verdade

**Conjunção (p ^ q)** — só V quando ambas são V:

| p | q | p ^ q |
|---|---|-------|
| V | V | V |
| V | F | F |
| F | V | F |
| F | F | F |

**Disjunção (p v q)** — só F quando ambas são F:

| p | q | p v q |
|---|---|-------|
| V | V | V |
| V | F | V |
| F | V | V |
| F | F | F |

## Relações

- [Paradigma Lógico](paradigma-logico.md) — aplica a lógica formal à programação
- [Linguagem Prolog](linguagem-prolog.md) — termos compostos como `homem(joao)`, `casados(joao,maria)`
- [Operadores e Expressões](operadores-e-expressoes.md) — operadores E/OU/NÃO e tabelas-verdade vistos em ALP (ponte entre disciplinas)

## Fontes

- [LP A13 — Programação Lógica: Conceitos](../fontes/lp-a13-programacao-logica-conceitos.md)
