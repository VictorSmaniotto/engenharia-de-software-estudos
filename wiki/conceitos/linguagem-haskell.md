---
titulo: Linguagem Haskell
tipo: conceito
tags: [linguagem, funcional, haskell, ml, funcional-puro, recursividade]
disciplina: Linguagens de Programação
fontes: [lp-a12-programacao-funcional-outras-linguagens]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Linguagem Haskell

## Definição

Linguagem **funcional pura** — sem variáveis nem atribuição, dependendo de [recursividade](recursividade.md) no lugar de laços. Similar à linguagem **ML**, mas com **sintaxe parecida com sistemas de equações matemáticas**, enquanto ML tem construção mais próxima das demais linguagens (LP A12; Sebesta, 2011).

## Haskell × ML (cálculo de fatorial)

| ML | Haskell |
|----|---------|
| `fun fact(n:int):int = if n=0 then 1 else n*fact(n-1);` | `fact 0 = 1`<br>`fact n = n * fact (n-1)` |

Ambos têm a função `fact`, uma **condição de parada** associada ao valor 0 e **chamadas recursivas** com redução de `n`. O diferencial de Haskell é expressar o caso base e o caso geral como **equações separadas** (estilo matemático).

## Relações

- [Paradigma Funcional](paradigma-funcional.md) — exemplo de funcional **puro** (ao lado de Haskell na tabela de linguagens)
- [Recursividade](recursividade.md) — obrigatória no funcional puro
- [Linguagem Scheme](linguagem-scheme.md) — funcional geral, em contraste

## Fontes

- [LP A12 — Programação Funcional: Outras Linguagens](../fontes/lp-a12-programacao-funcional-outras-linguagens.md)
