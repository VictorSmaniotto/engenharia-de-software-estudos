---
titulo: "ALP Aula 15 — Recursividade"
tipo: fonte
tags: [recursividade, sub-rotina, condicao-de-parada, potencia, tabuada]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-aula15-recursividade]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 15 — Recursividade

**Disciplina:** Algoritmos e Lógica de Programação  
**Módulo/Aula:** Aula 15  
**Data de ingestão:** 2026-06-15

---

## Resumo

Aprofunda o conceito de **recursividade**: uma sub-rotina que, em determinadas condições, chama a si mesma sucessivamente até atingir uma condição de parada. Compara a abordagem recursiva com a iterativa e apresenta dois exemplos práticos.

---

## Pontos-chave

- **Recursividade:** sub-rotina chama a si mesma; equivale funcionalmente a um laço de repetição, mas com lógica estruturada de forma distinta.
- **Condição de parada obrigatória:** sem ela, a recursão é infinita (equivalente a laço sem controle). O `SE` que verifica a condição-base é o mecanismo de encerramento.
- **Exemplo 1 — Potência recursiva:**
  ```
  FUNÇÃO POTENCIA (INTEIRO BASE, INTEIRO EXPOENTE) DE INTEIRO
    SE (EXPOENTE = 0) ENTÃO
      RETORNE 1;
    SENÃO
      RETORNE (BASE * POTENCIA(BASE, EXPOENTE-1));
    FIMSE;
  FIM;
  ```
  Cada chamada reduz o expoente em 1; base = 5, exp = 3 → 5 * (5 * (5 * 1)) = 125.
- **Versão iterativa equivalente:** mesmo resultado usando `PARA I DE 1 ATÉ EXPOENTE` com variável acumuladora `RESULTADO`. Mais simples de pensar, mas requer variáveis auxiliares.
- **Exemplo 2 — Tabuada recursiva:**
  Dois parâmetros: `VALOR1` (decrementado a cada chamada, controla iterações) e `VALOR2` (fixo, mantém o valor original da tabuada). O `ESCREVA` ocorre na *volta* das chamadas recursivas — tabuada exibida em ordem crescente apesar do decremento.
- **Quando usar recursão:** cálculos matemáticos com definição naturalmente recursiva; problemas que se dividem em subproblemas idênticos (ex.: fatorial, Fibonacci, busca em árvore).

---

## Conceitos relacionados

- [Recursividade](../conceitos/recursividade.md)
- [Sub-Rotinas](../conceitos/sub-rotinas.md)
- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md)

---

## Perguntas abertas

- O que acontece se a condição de parada nunca for atingida? (Stack overflow)
- Como a pilha de chamadas (call stack) suporta as chamadas recursivas?
