---
titulo: Linguagem Scheme
tipo: conceito
tags: [linguagem, funcional, scheme, lisp, lambda, define, recursividade]
disciplina: Linguagens de Programação
fontes: [lp-a12-programacao-funcional-outras-linguagens]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Linguagem Scheme

## Definição

Linguagem **funcional** criada na década de 1970, derivada de [Lisp](linguagem-lisp.md). Trata funções de forma mais flexível: podem ser **valores de expressões** ou **elementos de listas**, e assim servir como dados para variáveis ou parâmetros — recurso ausente na versão original de Lisp (Sebesta, 2011). Sintaxe e semântica simples, com **interpretador interativo**, tornam-na boa opção educacional (LP A12).

## Características sintáticas

- Expressões entre **parênteses** (delimitadores e controle de precedência), em [notação prefixa](notacao-prefixa.md).
- Operador sem operandos retorna o **elemento neutro**: `(+)` → 0; `(*)` → 1.
- Elemento primitivo retorna a si mesmo: `10` → 10.

```scheme
(* 2 (+ 1 3))   ; => 8
```

## Definição de funções

`define` associa um nome; `lambda` cria a função anônima:

```scheme
(define dobro (lambda (x) (* 2 x)))
(dobro 5)   ; => 10
```

## Entrada/saída e recursão

- E/S: `(read)`, `(display "...")`, `(newline)`.
- **Recursividade** com condição de parada (substitui laços):

```scheme
(define (fat n)
  (if (= n 0) 1 (* n (fat (- n 1)))))
```

## Relações

- [Linguagem Lisp](linguagem-lisp.md) — origem
- [Paradigma Funcional](paradigma-funcional.md) — funcional geral (agrega variáveis)
- [Recursividade](recursividade.md)
- [Notação Prefixa](notacao-prefixa.md)

## Fontes

- [LP A12 — Programação Funcional: Outras Linguagens](../fontes/lp-a12-programacao-funcional-outras-linguagens.md)
