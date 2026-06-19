---
titulo: Programação Dinâmica
tipo: conceito
tags: [paradigma, programacao-dinamica, grafos, otimizacao, estados, clojure]
disciplina: Linguagens de Programação
fontes: [lp-a15-outros-paradigmas]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Programação Dinâmica

## Definição

Forma de programação que **reduz problemas complexos a subproblemas de menor complexidade**, otimizando o desenvolvimento. Trata os problemas fracionados como completos, desde que seja possível **integrar as partes** numa solução para o problema original (LP A15).

## Aplicações

- Apoia-se na [Teoria de Grafos](teoria-de-grafos.md) (rotas logísticas) — representável como diagrama, **vetor** ou **matriz**.
- Adequada a problemas com baixa previsibilidade que exigem **adaptação a eventos**: controle de estoque (sobretudo e-commerce), rotas de GPS (recalculadas por acidentes, obras, erro do motorista).
- Trabalha com **estados** do processo: o que é necessário para o software operar conforme a dinâmica dos eventos.

## Linguagem associada

**[Clojure](linguagem-clojure.md)** aceita programação dinâmica: mesmo sendo tipada, os tipos **não são verificados na compilação**; como suas estruturas são listas, podem ser manipuladas em tempo de execução, interferindo nas funcionalidades em tempo real.

## Relações

- [Teoria de Grafos](teoria-de-grafos.md) — base para rotas e custos
- [Programação Orientada a Eventos](programacao-orientada-a-eventos.md) — adaptação a eventos
- [Linguagem Clojure](linguagem-clojure.md) — tipagem dinâmica
- [Vetores e Matrizes](vetores-e-matrizes.md) — representação de grafos

## Nota

O material apresenta "programação dinâmica" como **estilo de otimização adaptativa**. Distingue-se (ou ao menos não é detalhada) da técnica algorítmica clássica de mesmo nome (decomposição com memoização) — ver pergunta aberta em [LP A15](../fontes/lp-a15-outros-paradigmas.md).

## Fontes

- [LP A15 — Outros Paradigmas e Formas de Programação](../fontes/lp-a15-outros-paradigmas.md)
