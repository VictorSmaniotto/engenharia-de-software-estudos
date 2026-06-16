---
titulo: "ALP Aula 10 — Estruturas Homogêneas (Vetores)"
tipo: fonte
tags: [vetor, estrutura-homogenea, array, indice, busca]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula10-estruturas-homogeneas]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 10 — Estruturas Homogêneas (Vetores)

**Disciplina:** Algoritmo e Lógica de Programação  
**Módulo/Aula:** Aula 10  
**Data de ingestão:** 2026-06-15

---

## Resumo

Introduz as **estruturas de dados homogêneas unidimensionais** — vetores — como meio de armazenar listas de dados de um mesmo tipo sob um único identificador acessado por índice numérico.

---

## Pontos-chave

- **Estrutura homogênea:** todos os elementos têm o mesmo tipo; contraste com variáveis simples (um dado por vez).
- **Declaração (sintaxe Forbellone):**
  ```
  TIPO DADOS = VETOR [1..100] DE INTEIROS;
  DADOS: LISTA;
  ```
  A palavra `TIPO` define o tipo vetor; `LISTA` é a variável concreta.
- **Acesso por índice:** `LISTA[I]` — combinação do nome da estrutura com índice inteiro entre colchetes.
- **Preenchimento e busca com laços:** `PARA I DE 1 ATÉ 10` percorre sequencialmente todas as posições; `SE (LISTA[I] = BUSCA)` verifica igualdade em cada posição.
- **Variação eficiente:** substituir `PARA` por `ENQUANTO` na busca permite interromper iteração ao encontrar o valor (sem percorrer o restante do vetor).

---

## Conceitos relacionados

- [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md)
- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md)
- [Tipos de Dados](../conceitos/tipos-de-dados.md)

---

## Perguntas abertas

- Como garantir que o índice não ultrapasse os limites do vetor (out-of-bounds)?
- Qual a relação entre vetores em algoritmos e arrays em linguagens como C e Java?
