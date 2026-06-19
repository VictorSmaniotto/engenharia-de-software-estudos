---
titulo: Programação Orientada a Aspectos
tipo: conceito
tags: [paradigma, aspectos, aspectj, weaving, pointcut, java, kiczales]
disciplina: Linguagens de Programação
fontes: [lp-a15-outros-paradigmas]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Programação Orientada a Aspectos

## Definição

Forma de programação que organiza o código segundo sua **relevância** dentro dos requisitos da aplicação, complementando o [OO](paradigma-oo.md) (que se baseia em comportamentos de objetos). Permite encapsular código **secundário/transversal** em módulos separados chamados **aspectos**. Desenvolvida por [Gregor Kiczales](../autores/kiczales.md) e equipe na **Xerox PARC** (LP A15).

## AspectJ

Linguagem que **não cria aplicações completas**, mas **complementos para Java** (analogia: PHP/JavaScript ligados a HTML/CSS). Estrutura não contemplada pela linguagem Java pura, dando controle **transversal** de código.

- **`pointcut`**: desvio que contém o **`join point`** definindo a ligação entre classe e aspecto.
- **`call`**: referencia o método principal.
- **`before`**: executa o conteúdo do aspecto **antes** do método principal — comparado a um desvio incondicional, como o antigo **GOTO**.

## Aspect weaver e weaving

O **aspect weaver** age como um compilador: une o código principal a todos os aspectos pelo processo de **weaving**, gerando o *bytecode* interpretado pela máquina virtual Java.

## Aplicação típica

Agrupar em aspectos o tratamento de erros (abertura de arquivos, exceções diversas) e demais códigos transversais de menor relevância, mantendo o código principal limpo.

## Relações

- [Paradigma OO](paradigma-oo.md) — aspectos o complementam
- [Linguagem Java](linguagem-java.md) — AspectJ gera bytecode para a JVM
- [Compilação e Interpretação](compilacao-e-interpretacao.md) — weaving e bytecode
- [Gregor Kiczales](../autores/kiczales.md) — criador do paradigma

## Fontes

- [LP A15 — Outros Paradigmas e Formas de Programação](../fontes/lp-a15-outros-paradigmas.md)
