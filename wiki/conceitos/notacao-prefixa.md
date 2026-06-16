---
titulo: Notação Prefixa (Polonesa)
tipo: conceito
tags: [funcional, notacao-prefixa, notacao-polonesa, clojure, lisp]
disciplina: Linguagens de Programação
fontes: [lp-a10-programacao-funcional-conceitos, lp-a11-programacao-funcional-clojure]
criado: 2026-05-19
atualizado: 2026-05-19
---

# Notação Prefixa (Polonesa)

## Definição

A **notação prefixa** (também chamada **notação polonesa**) é uma forma de escrever expressões matemáticas e lógicas em que o **operador vem antes dos operandos**. É a notação padrão do paradigma funcional, oposta à notação **infixa** usada em linguagens imperativas.

## Comparação

| Notação | Exemplo | Usada em |
|---------|---------|----------|
| **Infixa** (convencional) | `3 + 4` | C, Java, Python, etc. |
| **Prefixa** (polonesa) | `(+ 3 4)` | Lisp, Clojure, Scheme |

## No contexto do paradigma funcional

Em Lisp e Clojure, as expressões são escritas como listas onde:
- O **primeiro elemento** é a função/operador
- Os **demais elementos** são os argumentos

```clojure
(+ 3 4)           ; soma: 3 + 4 = 7
(* 5 2)           ; produto: 5 * 2 = 10
(/ (apply + nums) (count nums))  ; média aritmética
```

As funções primitivas também seguem a mesma lógica:
```clojure
(defn media [numeros]      ; define função "media" com parâmetro "numeros"
  (/ (apply + numeros) (count numeros)))
```

## Uso fora da programação

A notação polonesa é utilizada em **calculadoras financeiras** (ex.: HP-12C) — o operador é inserido após os operandos em sua variante RPN (*Reverse Polish Notation*, ou pós-fixa).

## Por que essa notação?

- Elimina ambiguidade de precedência de operadores (não precisa de parênteses extras para grupos)
- Permite que funções e operadores sejam tratados de forma uniforme
- Toda chamada de função segue o mesmo padrão: `(função arg1 arg2 ...)`

## Relações

- [Paradigma Funcional](paradigma-funcional.md) — contexto do paradigma
- [Linguagem Clojure](linguagem-clojure.md) — uso prático da notação
- [Funções Puras e Imutabilidade](funcoes-puras.md) — conceito central do funcional

## Fontes

- [LP A10 — Programação Funcional: Conceitos](../fontes/lp-a10-programacao-funcional-conceitos.md)
- [LP A11 — Programação Funcional: Linguagem Clojure](../fontes/lp-a11-programacao-funcional-clojure.md)
