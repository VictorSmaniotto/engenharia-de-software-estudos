---
titulo: LP A12 — Programação Funcional: Outras Linguagens
tipo: fonte
tags: [linguagens, funcional, lisp, scheme, haskell, ml, kotlin, python, recursividade]
disciplina: Linguagens de Programação
fontes: [lp-a12-programacao-funcional-outras-linguagens]
criado: 2026-06-18
atualizado: 2026-06-18
---

# LP A12 — Programação Funcional: Outras Linguagens

- **Disciplina:** Linguagens de Programação
- **Aula:** 12 — Programação Funcional: Outras Linguagens
- **Fonte original:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-12.html
- **Ingerida em:** 2026-06-18

## Resumo

A aula percorre linguagens representativas do [paradigma funcional](../conceitos/paradigma-funcional.md), partindo da pioneira **Lisp** e de sua derivada **Scheme**, e mostrando como o funcional aparece tanto em linguagens puras (**Haskell**, **ML**) quanto em linguagens multiparadigma modernas (**Kotlin**, **Python**, **Java 8+**). O fio condutor é a construção de código como **funções delimitadas por parênteses** em notação prefixa, e o papel central da **recursividade** no lugar de laços.

## Pontos-chave

- **Lisp** é a linguagem funcional mais antiga; usa dois tipos de estrutura: **átomos** (elementos puros — letras, números) e **listas** (conjuntos de átomos e/ou listas, que também podem ser elementos de outra lista). Funções em notação prefixa: `(+ 5 5)` → 10; aninhamento `(* 2 (- 10 5))` → 10. Apesar da evolução, nunca alcançou grande popularidade de mercado pelas limitações práticas.
- **Kotlin** (JetBrains) é multiparadigma: base orientada a objetos, mas por permitir **funções fora de classes** pode implementar código puramente funcional. Voltada a web, mobile e desktop.
- **Scheme** (década de 1970) deriva de Lisp e trata funções de forma mais flexível: podem ser **valores de expressões ou elementos de listas**, servindo como dados para variáveis ou parâmetros — recurso que a versão original de Lisp não oferecia (Sebesta, 2011). Sintaxe simples; interpretador interativo, bom para uso educacional.
- Exemplos Scheme: elementos primitivos retornam a si mesmos (`10` → 10); operador sem operandos retorna o **elemento neutro** (`(+)` → 0; `(*)` → 1); precedência controlada por parênteses (`(* 2 (+ 1 3))` → 8).
- `define` associa nome a uma função; `lambda` cria a função anônima: `(define dobro (lambda (x) (* 2 x)))`. Entrada/saída: `(read)`, `(display ...)`, `(newline)`.
- **Recursividade** no funcional não difere muito da imperativa: exige uma estrutura de decisão com **condição de parada**, e a cada iteração a função se aproxima dessa condição. Ex. fatorial em Scheme: `(define (fat n) (if (= n 0) 1 (* n (fat (- n 1)))))`.
- **Haskell** é funcional **puro**, similar a **ML**, mas com sintaxe parecida com sistemas de equações matemáticas. Comparação (Sebesta, 2011): ML usa `fun fact(n:int):int = if n=0 then 1 else n*fact(n-1)`; Haskell usa `fact 0 = 1` / `fact n = n * fact (n-1)`.
- **Python** e **Java (8+)** agregam o funcional ao orientado a objetos. Python usa o multiparadigma de forma natural, com sintaxe limpa (ex.: `def par(x): return (x % 2) == 0`).

## Conexões com a wiki

- Detalha o [Paradigma Funcional](../conceitos/paradigma-funcional.md) já introduzido em LP A2 e A10.
- Origina as páginas de conceito [Linguagem Lisp](../conceitos/linguagem-lisp.md), [Linguagem Scheme](../conceitos/linguagem-scheme.md), [Linguagem Haskell](../conceitos/linguagem-haskell.md) e [Linguagem Kotlin](../conceitos/linguagem-kotlin.md).
- Reforça [Notação Prefixa](../conceitos/notacao-prefixa.md) e [Recursividade](../conceitos/recursividade.md) (substituição de laços no funcional puro).
- Lisp como base histórica da IA conecta-se à nota histórica do [Paradigma Funcional](../conceitos/paradigma-funcional.md).

## Perguntas abertas

- Como Scheme/Lisp tratam recursão de cauda e otimização para iteração na prática?
- Quais limitações concretas de mercado travaram a adoção de Lisp?
