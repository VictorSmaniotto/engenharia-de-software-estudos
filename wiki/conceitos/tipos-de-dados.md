---
titulo: Tipos de Dados
tipo: conceito
tags: [tipos-de-dados, inteiro, real, caractere, logico, algoritmo]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a05-tipos-de-dados]
criado: 2026-05-28
atualizado: 2026-05-28
---

# Tipos de Dados

## Definição

Tipos de dados definem quais valores uma estrutura de dados pode armazenar e quais operações podem ser realizadas sobre eles. Em algoritmos, toda variável deve ter seu tipo declarado antes de ser utilizada.

---

## Tipos Básicos

| Tipo | Descrição | Exemplos |
|------|-----------|---------|
| `INTEIRO` | Números sem casas decimais (positivos ou negativos) | `20`, `-5`, `0` |
| `REAL` | Números com casas decimais | `50.5`, `3.14`, `-2.7` |
| `CARACTERE` | Um caractere simples ou uma cadeia de caracteres (string) | `'A'`, `"RONIE"` |
| `LÓGICO` | Apenas dois estados: verdadeiro ou falso | `VERDADEIRO`, `FALSO` |

A base de todos os dados são os **bits**; os tipos de dados mais complexos (imagens, sons, estruturas heterogêneas) são construídos sobre os tipos básicos.

---

## Tipagem em Algoritmos

- Toda variável deve ter seu tipo definido na declaração (tipagem estática)
- Declarar variável sem tipo é possível, mas não recomendado: o tipo só será definido quando o primeiro dado for inserido, reduzindo a previsibilidade e aumentando o risco de erros
- O tipo determina quais operadores podem ser aplicados (ex: operadores matemáticos em INTEIRO e REAL; operadores lógicos em LÓGICO)

---

## Relações

- [Variáveis e Constantes](variaveis-e-constantes.md) — variáveis são declaradas associadas a um tipo
- [Operadores e Expressões](operadores-e-expressoes.md) — o tipo do resultado de uma expressão depende dos tipos dos operandos
- [Pseudocódigo](pseudocodigo.md) — a declaração de tipos faz parte da sintaxe do pseudocódigo (`DECLARE`)
- [Escopo](escopo.md) — ciclo de vida dos dados tipados durante a execução

## Fontes

- [ALP A05 — Tipos de Dados](../fontes/alp-a05-tipos-de-dados.md)
- [Forbellone (2005)](../autores/forbellone.md)
