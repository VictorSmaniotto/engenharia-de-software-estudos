---
titulo: "ALP Aula 09 — Aninhamento de Estruturas"
tipo: fonte
tags: [aninhamento, estruturas-de-controle, teste-de-mesa, decisao, repeticao]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-aula09-aninhamento-estruturas]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 09 — Aninhamento de Estruturas

**Disciplina:** Algoritmos e Lógica de Programação  
**Módulo/Aula:** Aula 09  
**Data de ingestão:** 2026-06-15

---

## Resumo

A aula apresenta como estruturas de controle (decisão e repetição) podem ser combinadas — aninhadas umas dentro das outras — para resolver problemas com maior complexidade lógica. Introduz o **teste de mesa** como ferramenta de validação de algoritmos.

---

## Pontos-chave

- **Aninhamento de Estruturas de Decisão:** um `SE` dentro de outro `SE`; a estrutura interna só é avaliada se a externa resultar `VERDADEIRO`. Exemplo: determinar o maior entre três variáveis.
- **Teste de Mesa (Manzano, 1997):** tabela com amostras de dados para simular a execução do algoritmo e detectar falhas; colunas = variáveis de entrada + resultado esperado.
- **Aninhamento de Estruturas de Repetição:** dois ou mais `PARA` encadeados; contador interno completa ciclo inteiro antes de o externo avançar. Exemplo clássico: hodômetro de três dígitos (000–999).
- **Repetição dentro de Decisão:** laço só é acionado se condição `SE` for satisfeita.
- **Decisão dentro de Repetição:** estrutura `SE` avaliada a cada iteração; permite alterar variável de controle do laço para forçar encerramento antecipado.

---

## Conceitos relacionados

- [Estruturas de Decisão](../conceitos/estruturas-de-decisao.md)
- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md)
- [Aninhamento de Estruturas](../conceitos/aninhamento-de-estruturas.md)

---

## Perguntas abertas

- Qual é o limite prático de níveis de aninhamento antes de prejudicar legibilidade?
- Como o teste de mesa se relaciona com os casos de teste em engenharia de software?
