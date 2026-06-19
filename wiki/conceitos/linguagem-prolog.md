---
titulo: Linguagem Prolog
tipo: conceito
tags: [linguagem, logico, prolog, fatos, regras, instancias, comutatividade, sistemas-especialistas]
disciplina: Linguagens de Programação
fontes: [lp-a14-programacao-logica-prolog]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Linguagem Prolog

## Definição

Linguagem representativa do [Paradigma Lógico](paradigma-logico.md). Trabalha com **fatos** sobre objetos e **regras/relações** entre eles, além de variáveis, listas e recursividade. A proposta é declarar **o que serve de base** para o processamento, não **como** processar (LP A14).

## Fatos, relações e instâncias

- **Proposições atômicas**: relações que incidem sobre **termos** (equivalentes aos átomos de [Lisp](linguagem-lisp.md)), em listas entre parênteses separadas por vírgulas.
- Cada linha é uma **instância**; o conjunto de instâncias **define a relação**.

```prolog
amigo(ana, marcos).
amigo(ana, silvio).
amigo(paulo, victor).
```

## Sintaxe de termos

- **Constantes**: iniciam com letra **minúscula** (`ana`, `marcos`).
- **Variáveis**: iniciam com letra **maiúscula** (`X`, `Y`, `Media`).

## Comutatividade

O interpretador **não entende o sentido do nome** da relação — só as instâncias importam. `amigo` é comutativa, mas se `marcos` só aparece como segundo termo, `? amigo(marcos, Y).` retorna `false`. Corrige-se **adicionando as instâncias com termos invertidos**. Já `pai`, `mae` e `chefe` **não** são comutativas.

## Consultas e cálculos

```prolog
? amigo(X, Y).            % lista todas as instâncias
? pessoa(X,Y,Z), Media is Z/Y.   % cálculo em tempo de execução
```

A consulta de árvore genealógica (`pai`, `mae`, `irmãos`) mostra `irmãos` aparecendo duas vezes pela comutatividade.

## Aplicações

Computação simbólica (prova automática de teoremas), bancos de dados relacionais, linguagem natural, solucionadores de jogos e **sistemas especialistas**. Plataforma de teste: SWISH (swish.swi-prolog.org).

## Relações

- [Paradigma Lógico](paradigma-logico.md) — Prolog é seu principal representante
- [Lógica Formal](logica-formal.md) — base de proposições e relações
- [Linguagem Lisp](linguagem-lisp.md) — termos × átomos
- [Recursividade](recursividade.md) — suportada pela linguagem

## Fontes

- [LP A14 — Programação Lógica: Linguagem Prolog](../fontes/lp-a14-programacao-logica-prolog.md)
