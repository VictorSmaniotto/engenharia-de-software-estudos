---
titulo: Paradigma Lógico (Programação Lógica)
tipo: conceito
tags: [paradigma, logico, prolog, regras, fatos, declarativo, nao-procedural, logica-formal, IA]
disciplina: Linguagens de Programação
fontes: [lp-a02-classificacao-de-paradigmas, lp-a13-programacao-logica-conceitos, lp-a14-programacao-logica-prolog]
criado: 2026-05-07
atualizado: 2026-06-18
---

# Paradigma Lógico

## Definição

Uma das três categorias principais de paradigmas segundo Sebesta (2011). Fundamenta-se na [Lógica Formal](logica-formal.md): programas são conjuntos de **fatos** e **regras** (proposições) **sem ordem de execução predefinida**, formando uma base de conhecimento que pode ser consultada para inferir novas informações.

> "As regras que servem de base são definidas sem uma ordem lógica e podem ser acessadas livremente de forma que sirvam como uma base complexa de informações que podem ser utilizadas na geração de novas informações." (LP A2)

## Declarativo e não-procedural

- **Declarativo**: descreve-se **o que é verdade** (fatos e relações), não *como* chegar ao resultado. Mais simples em semântica que o imperativo, porém com **menor variedade de soluções computacionais** — daí mais limitado no mercado.
- **Não-procedural**: foca na **forma do resultado**, não no processamento. O programador tem menos controle sobre a sequência de ações.

| | Procedural (imperativo) | Não-procedural (lógico) |
|---|---|---|
| O que se descreve | Sequência de ações sobre os dados | Características dos elementos e relações entre eles |
| Controle do processo | Total (passo a passo) | Delegado ao motor de inferência |

## Estruturas

- **Proposições atômicas**: combinação de símbolos de predicados com termos simples/compostos entre parênteses.
- **Termos compostos** representam funções (sintaxe similar à do funcional). Ex.: `homem(joao).`, `mulher(maria).`, `casados(joao,maria).` — os dois primeiros são **fatos**; o terceiro, uma relação entre dois elementos.

## Contraste com o imperativo

No [imperativo](paradigma-imperativo.md), o programador define *como* chegar ao resultado. No lógico, define *o que é verdade* (regras e fatos) e o sistema infere o resultado.

## Linguagem representativa

[**Prolog**](linguagem-prolog.md) — fatos, regras, instâncias, comutatividade, variáveis e listas. Citada desde LP A1 como linguagem para IA, junto com Lisp e Scheme.

## Aplicações

- Índices e relações algébricas em **bancos de dados** (grandes volumes).
- **Inteligência artificial e aprendizado de máquina**: gerar novo conhecimento a partir de novas relações entre proposições existentes.

## Relações

- [Lógica Formal](logica-formal.md) — base matemática
- [Linguagem Prolog](linguagem-prolog.md) — principal representante
- [Paradigma Imperativo](paradigma-imperativo.md) — contraste declarativo × procedural
- [Paradigma Funcional](paradigma-funcional.md) — também não-imperativo; sintaxe de relações lembra funções

## Fontes

- [LP A2 — Classificação de Paradigmas](../fontes/lp-a02-classificacao-de-paradigmas.md)
- [LP A13 — Programação Lógica: Conceitos](../fontes/lp-a13-programacao-logica-conceitos.md)
- [LP A14 — Programação Lógica: Linguagem Prolog](../fontes/lp-a14-programacao-logica-prolog.md)
- [LP M2 A1 — Paradigmas de Programação](../fontes/lp-m2-a01-paradigmas-de-programacao.md)
