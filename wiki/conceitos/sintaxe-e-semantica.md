---
titulo: Sintaxe e Semântica
tipo: conceito
tags: [sintaxe, semantica, compilacao, linguagens]
disciplina: Linguagens de Programação
fontes: [lp-a03-programacao-estruturada-conceitos]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Sintaxe e Semântica

## Definição

**Sintaxe** é a forma correta de construção de cada instrução: a combinação exata de palavras reservadas, operadores e parâmetros que torna um comando válido para a linguagem.

**Semântica** complementa a sintaxe com um olhar mais amplo: avalia se o código está estruturado de forma lógica e coerente dentro dos paradigmas da linguagem — se as instruções estão nos lugares certos, independentemente de estarem sintaticamente corretas.

> "A semântica se refere à construção do código em si, observando a correta colocação das instruções em seus devidos lugares, estejam elas corretas ou não, pois essa outra preocupação é função da sintaxe." (LP A3)

## Papel no Processo de Compilação

| Etapa | Verificação | Ferramenta |
|-------|-------------|------------|
| Análise léxica | Caracteres → lexemas (tokens) | Analisador léxico |
| Análise **sintática** | Tokens → árvore léxica; comandos bem formados | Analisador sintático (Sebesta, 2011) |
| Análise **semântica** | Estrutura completa do código; instruções no lugar certo | Analisador semântico |

## Limitações

Nem todo erro é detectável em tempo de compilação/análise. Erros de lógica ou uso incorreto de comandos para certas ações só aparecem em execução e teste.

## Relações

- [Compilação e Interpretação](compilacao-e-interpretacao.md) — processo que aplica sintaxe e semântica para transformar código
- [Linguagem C](linguagem-c.md) — exemplo com semântica estruturada em funções e delimitadores explícitos

## Fontes

- [LP A3 — Programação Estruturada: Conceitos](../fontes/lp-a03-programacao-estruturada-conceitos.md)
