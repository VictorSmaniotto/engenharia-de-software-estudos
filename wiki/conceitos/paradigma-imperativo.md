---
titulo: Paradigma Imperativo
tipo: conceito
tags: [paradigma, imperativo, estruturado, procedural]
disciplina: Linguagens de Programação
fontes: [lp-a02-classificacao-de-paradigmas, lp-a03-programacao-estruturada-conceitos]
criado: 2026-05-07
atualizado: 2026-05-11
---

# Paradigma Imperativo

## Definição

Uma das três categorias principais de paradigmas segundo Sebesta (2011). Define programas como sequências ordenadas de instruções que modificam o estado do programa ao longo da execução.

> Linguagens imperativas possuem "uma ordem lógica para a execução de uma grande variedade de estruturas que podem ser organizadas como independentes ou dependentes umas das outras, mas tendo uma ordem planejada de execução." (LP A2)

## Derivações e subtipos

- **Estruturado** — forma clássica do imperativo; ver [Paradigma Estruturado](paradigma-estruturado.md)
- **Orientado a Objetos** — derivação do imperativo com foco em abstração de dados; ver [Paradigma OO](paradigma-oo.md)
- **Scripts** — JavaScript, Ruby, Perl são "basicamente imperativos" (LP A2)
- **Linguagens visuais** — Visual Basic, Delphi derivam de imperativos textuais (C, Basic, Pascal)

## Linguagens representativas

C, Pascal, BASIC, Fortran, COBOL, Python, Java, JavaScript, Ruby, Perl, Visual Basic, Delphi

## Contraste com outros paradigmas

| Paradigma | Mutabilidade de estado | Ordem de execução |
|-----------|----------------------|-------------------|
| **Imperativo** | Alta (estados mudam constantemente) | Ordenada e planejada |
| [Funcional](paradigma-funcional.md) | Baixa (imutabilidade) | Avaliação de expressões |
| [Lógico](paradigma-logico.md) | — | Sem ordem definida |

## Origens: Máquina de Turing

A ideia base do paradigma imperativo foi a **Máquina de Turing**, concebida pelo matemático britânico **Alan Turing** ("pai da computação"). A máquina operava com: unidade lógica/aritmética, unidade de controle, unidade de E/S e memória primária — formando a tríade entrada → processamento → saída que é fundamento da computação.

## Comando GOTO

Na forma mais primitiva do imperativo (antes do estruturado), o fluxo de execução era controlado pelo comando **GOTO**: desviava a execução para marcadores numéricos ou textuais inseridos no código. Ausência de sub-rotinas tornava o código um bloco único com desvios internos (ver exemplo em BASIC em [LP A3](../fontes/lp-a03-programacao-estruturada-conceitos.md)).

## Fontes

- [LP A2 — Classificação de Paradigmas](../fontes/lp-a02-classificacao-de-paradigmas.md)
- [LP A3 — Programação Estruturada: Conceitos](../fontes/lp-a03-programacao-estruturada-conceitos.md)
