---
titulo: "ALP Aula 13 — Sub-Rotinas (Procedimentos e Funções)"
tipo: fonte
tags: [sub-rotina, procedimento, funcao, escopo, paradigma-estruturado, modularizacao]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula13-sub-rotinas]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 13 — Sub-Rotinas (Procedimentos e Funções)

**Disciplina:** Algoritmo e Lógica de Programação  
**Módulo/Aula:** Aula 13  
**Data de ingestão:** 2026-06-15

---

## Resumo

Introduz o **paradigma estruturado** via sub-rotinas — blocos de código nomeados que podem ser chamados a partir do algoritmo principal ou de outras sub-rotinas. Distingue **procedimentos** (sem retorno) de **funções** (com retorno). Define escopo global e local.

---

## Pontos-chave

- **Sub-rotina:** trecho de código com nome próprio e certa independência funcional; pode ser chamado várias vezes sem duplicar código (reuso).
- **Escopo de estruturas de dados:**
  - **Global:** declarada no algoritmo principal; acessível de qualquer ponto.
  - **Local:** declarada dentro de uma sub-rotina; inacessível externamente; perdida ao sair da sub-rotina.
- **Procedimento:** sub-rotina sem retorno de valor; acessa globais diretamente; chamado pelo nome.
  ```
  PROCEDIMENTO CALCULA ()
    DECLARE INTEIRO: SOMA;
    SOMA <- V1 + V2 + V3;
    ESCREVA ("RESULTADO = ", SOMA);
  FIM;
  ```
- **Função:** sub-rotina com tipo de retorno; usa `RETORNE` ao final; deve ser atribuída a uma variável, usada em expressão ou em `ESCREVA`.
  ```
  FUNÇÃO CALCULA () DE INTEIRO
    DECLARE INTEIRO: SOMA;
    SOMA <- V1 + V2 + V3;
    RETORNE SOMA;
  FIM;
  ```
- **Autores:** Forbellone (2005) usa o termo "módulo" para toda sub-rotina; Manzano (1997) distingue procedimentos de funções — convenção adotada no material.

---

## Conceitos relacionados

- [Sub-Rotinas](../conceitos/sub-rotinas.md)
- [Escopo](../conceitos/escopo.md)
- [Paradigma Estruturado](../conceitos/paradigma-estruturado.md)

---

## Perguntas abertas

- Como o conceito de sub-rotina se diferencia do de método em OO?
- Quando preferir procedimento em vez de função?
