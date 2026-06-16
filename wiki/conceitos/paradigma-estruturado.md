---
titulo: Paradigma Estruturado (Programação Estruturada)
tipo: conceito
tags: [paradigma, estruturado, procedural, sub-rotinas, funcoes]
disciplina: Linguagens de Programação
fontes: [lp-m2-a01-paradigmas-de-programacao, lp-a03-programacao-estruturada-conceitos, lp-a04-programacao-estruturada-linguagem-c]
criado: 2026-05-07
atualizado: 2026-05-11
---

# Paradigma Estruturado

## Definição

Evolução direta do [Paradigma Imperativo](paradigma-imperativo.md): mantém sua base (sequência de instruções que alteram estado) e acrescenta estruturas organizacionais mais complexas. É o paradigma "mais popular da história do desenvolvimento de código, presente até os dias atuais em grande parte das linguagens de programação." (LP A3)

## O que Acrescenta ao Imperativo

| Recurso | Imperativo puro | Estruturado |
|---------|----------------|-------------|
| Fluxo de controle | GOTO (desvio para marcadores) | `if/else`, `while`, `for` em blocos |
| Organização do código | Bloco único | Sub-rotinas independentes (funções/procedimentos) |
| Reúso de código | Baixo | Alto (funções reutilizáveis) |
| Portabilidade | Não prioritária | Começou a ser considerada |

## Conceitos-chave do Paradigma

- **Sub-rotinas / Funções**: blocos de código independentes que trocam dados por parâmetros; permitem reúso e melhor legibilidade
- **Estruturas de decisão**: `if/else` — desvio condicional baseado em expressão lógica
- **Laços de repetição**: `while`, `for` — blocos executados enquanto uma condição for verdadeira
- **Aninhamento**: estruturas encadeadas dentro de outras (ex.: `if` dentro de `while`)
- **Bibliotecas**: arquivos com código pré-desenvolvido e testado, importados conforme necessidade

## Surgimento e Linguagens

- Conceito surgiu na **década de 1950**; primeiras implementações: Algol, COBOL
- Linguagens estruturadas puras: Pascal, C, BASIC (versões originais), PHP, Perl, Go
- Linguagens que partiram do estruturado e absorveram OO: Java, C++, Python

## Linguagem Canônica

A [Linguagem C](linguagem-c.md) é considerada o exemplo mais representativo: cobre baixo e alto nível, tem sintaxe explícita com delimitadores (`{ }`, `;`), e toda execução parte de uma função `main()`.

## Relações

- [Paradigma Imperativo](paradigma-imperativo.md) — base do estruturado
- [Orientação a Objetos](paradigma-oo.md) — paradigma que surgiu como evolução/alternativa ao estruturado
- [Linguagem C](linguagem-c.md) — linguagem canônica do estruturado
- [Sintaxe e Semântica](sintaxe-e-semantica.md) — análise de código estruturado
- [Compilação e Interpretação](compilacao-e-interpretacao.md) — linguagens estruturadas são frequentemente compiladas
- [Escopo](escopo.md), [Ponteiros](ponteiros.md), [Vetores e Matrizes](vetores-e-matrizes.md) — conceitos práticos em C

## Fontes

- [LP M2 A1 — Paradigmas de Programação](../fontes/lp-m2-a01-paradigmas-de-programacao.md)
- [LP A3 — Programação Estruturada: Conceitos](../fontes/lp-a03-programacao-estruturada-conceitos.md)
- [LP A4 — Programação Estruturada: Linguagem C](../fontes/lp-a04-programacao-estruturada-linguagem-c.md)
- [ALP A2 — Classificação de Algoritmos](../fontes/alp-a02-classificacao-de-algoritmos.md) _(exemplo de pseudocódigo estruturado com PROCEDIMENTO)_
