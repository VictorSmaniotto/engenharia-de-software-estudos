---
titulo: Programação Orientada a Eventos
tipo: conceito
tags: [paradigma, eventos, gui, gatilhos, design-patterns, arduino, blocos]
disciplina: Linguagens de Programação
fontes: [lp-a15-outros-paradigmas]
criado: 2026-06-18
atualizado: 2026-06-18
---

# Programação Orientada a Eventos

## Definição

Paradigma alternativo em que o software reage a **eventos** por meio de rotinas de tratamento de **gatilhos** acionados por mecanismos de entrada, por outros softwares ou pelo sistema operacional. Não é necessariamente extensão do [OO](paradigma-oo.md), mas pode usar seus conceitos (ex.: C#) (LP A15).

## Características

- Fluxo de execução **descontínuo**: há uma **rotina principal que aguarda eventos** e é interrompida para tratá-los, retornando depois ao estado de espera. Difere do imperativo/OO, cujo fluxo é determinado pelo processamento dos dados.
- Eventos podem ser previsíveis ou não, com ou sem interação humana (cliques, teclas, toques, entradas automatizadas) — e podem **nunca ocorrer**.
- Eventos **esperados** são tratados pelo software; **inesperados**, pelo sistema operacional. Quanto mais completo o tratamento, mais robusta a aplicação.
- Usa *design patterns* (modelos de solução testados, não código pronto).

## Exemplos

- GUIs desktop: Visual Basic, Visual C, Delphi.
- Eventos em formulários web: C#, [Java](linguagem-java.md), JavaScript.
- **Arduino** (versão própria de C): laço infinito `loop()` interrompido por eventos/interrupções; `setup()` configura a placa.
- **Programação em blocos** (Scratch, Blockly): montagem gráfica por encaixe, didática para ensinar lógica do [paradigma imperativo](paradigma-imperativo.md); blocos podem ser traduzidos para outras linguagens.

## Relações

- [Paradigma OO](paradigma-oo.md) — pode usar seus conceitos
- [Paradigma Imperativo](paradigma-imperativo.md) — contraste de fluxo de execução
- [Programação Dinâmica](programacao-dinamica.md) — sistemas que se adaptam a eventos

## Fontes

- [LP A15 — Outros Paradigmas e Formas de Programação](../fontes/lp-a15-outros-paradigmas.md)
