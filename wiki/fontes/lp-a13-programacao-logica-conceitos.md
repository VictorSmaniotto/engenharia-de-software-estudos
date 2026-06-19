---
titulo: LP A13 — Programação Lógica: Conceitos
tipo: fonte
tags: [linguagens, logico, logica-formal, proposicoes, operadores-logicos, declarativo, prolog]
disciplina: Linguagens de Programação
fontes: [lp-a13-programacao-logica-conceitos]
criado: 2026-06-18
atualizado: 2026-06-18
---

# LP A13 — Programação Lógica: Conceitos

- **Disciplina:** Linguagens de Programação
- **Aula:** 13 — Programação Lógica: Conceitos
- **Fonte original:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-13.html
- **Ingerida em:** 2026-06-18

## Resumo

A aula fundamenta o [paradigma lógico](../conceitos/paradigma-logico.md) na **lógica formal** (ramo da matemática). Apresenta proposições simples e compostas, os operadores lógicos e suas tabelas-verdade, e mostra como esses conceitos se adaptam à programação. Conclui caracterizando o paradigma lógico como **declarativo** e **não-procedural**, contrastando-o com linguagens procedurais.

## Pontos-chave

- **Lógica formal** (Sebesta, 2011): conceito fundamental são as **proposições** — sentenças lógicas que resultam verdadeiras ou falsas, construídas a partir de relacionamentos entre elementos.
- Elementos podem ser **constantes** (símbolo que representa um objeto), **variáveis** (símbolo que representa objetos diferentes em momentos diferentes — mais próximas das variáveis da matemática que das de uma linguagem imperativa) ou termos.
- **Proposição simples**: uma única avaliação V/F. **Proposição composta**: combina proposições simples por meio de **operadores lógicos**.
- Operadores da lógica: negação, conjunção, disjunção, equivalência, implicação — nem todos com os mesmos símbolos/uso da programação. Expressões como "a ⊃ b" (implicação) e "a ∩ b" são comuns na matemática de conjuntos e correspondem às operações **E** e **OU**.
- **Tabela-verdade da conjunção (p ^ q)**: só resulta V quando ambas as proposições são V. **Disjunção (p v q)**: só resulta F quando ambas são F.
- **Termos compostos** são representações de funções (sintaxe similar a outros paradigmas) e formam as principais estruturas das linguagens lógicas. Ex.: `homem(joao).`, `mulher(maria).`, `casados(joao,maria).` — os dois primeiros são **fatos**; o terceiro relaciona dois elementos.
- **Proposições atômicas**: combinação de símbolos de predicados com termos simples/compostos entre parênteses.
- Linguagens lógicas são **declarativas**: mais simples que as imperativas em semântica, porém com menor variedade de soluções computacionais — daí mais limitadas no mercado.
- Por serem **não-procedurais**, focam na **forma do resultado**, não no processamento em si; o programador tem menos controle sobre a sequência de ações do que no imperativo. Em linguagens procedurais, um algoritmo aplica uma sequência de ações sobre os dados; nas não-procedurais, descrevem-se apenas as **características dos elementos e as relações entre eles**.
- Aplicações: índices em **bancos de dados** e relações algébricas para grandes volumes; **inteligência artificial e aprendizado de máquina** (gerar novo conhecimento a partir de novas relações entre proposições existentes).

## Conexões com a wiki

- Expande substancialmente o [Paradigma Lógico](../conceitos/paradigma-logico.md), antes só esboçado em LP A2.
- Origina o conceito [Lógica Formal](../conceitos/logica-formal.md).
- Os operadores lógicos e tabelas-verdade dialogam com [Operadores e Expressões](../conceitos/operadores-e-expressoes.md) (ALP), criando ponte entre disciplinas.
- Prepara a aula seguinte sobre [Linguagem Prolog](../conceitos/linguagem-prolog.md).

## Perguntas abertas

- Como a equivalência e a implicação se manifestam (se manifestam) em Prolog?
- Em que medida bancos de dados relacionais herdam do paradigma lógico?
