---
titulo: Linguagem Lisp
tipo: conceito
tags: [linguagem, funcional, lisp, atomos, listas, notacao-prefixa, ia]
disciplina: Linguagens de Programação
fontes: [lp-a12-programacao-funcional-outras-linguagens, lp-m2-a01-paradigmas-de-programacao]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Linguagem Lisp

## Definição

Linguagem **funcional mais antiga** (década de 1950–60), criada com foco em **Inteligência Artificial**. É a base histórica do [Paradigma Funcional](paradigma-funcional.md) e influenciou diretamente [Scheme](linguagem-scheme.md) e [Clojure](linguagem-clojure.md). Evoluiu ao longo do tempo, mas nunca alcançou grande popularidade de mercado devido a limitações em aplicações práticas (LP A12).

## Estruturas de dados (versão original)

Apenas dois tipos:
- **Átomos** — elementos puros: letras ou números.
- **Listas** — conjuntos formados por átomos e/ou listas (uma lista pode ser elemento de outra lista). Delimitadas por parênteses.

## Sintaxe de funções

Usa [Notação Prefixa](notacao-prefixa.md): o operador (função matemática) é o **primeiro átomo** dentro dos parênteses, seguido dos operandos.

```
(+ 5 5)        ; => 10
(* 2 (- 10 5)) ; => 10  (funções aninhadas)
```

## Relações

- [Paradigma Funcional](paradigma-funcional.md) — Lisp é sua origem
- [Linguagem Scheme](linguagem-scheme.md) — derivada direta de Lisp
- [Linguagem Clojure](linguagem-clojure.md) — Lisp moderno na JVM
- [Notação Prefixa](notacao-prefixa.md)
- Nota histórica: base para os estudos iniciais de IA — ver [Paradigma Funcional](paradigma-funcional.md)

## Fontes

- [LP A12 — Programação Funcional: Outras Linguagens](../fontes/lp-a12-programacao-funcional-outras-linguagens.md)
- [LP M2 A1 — Paradigmas de Programação](../fontes/lp-m2-a01-paradigmas-de-programacao.md)
