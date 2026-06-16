---
titulo: "ALP Aula 14 — Parâmetros em Sub-Rotinas"
tipo: fonte
tags: [parametro, argumento, passagem-por-valor, passagem-por-referencia, sub-rotina]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula14-parametros]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 14 — Parâmetros em Sub-Rotinas

**Disciplina:** Algoritmo e Lógica de Programação  
**Módulo/Aula:** Aula 14  
**Data de ingestão:** 2026-06-15

---

## Resumo

Apresenta os dois mecanismos de **passagem de parâmetros** entre partes de um algoritmo: por valor (cópia) e por referência (ponteiro ao dado original). Resolve o problema de comunicação entre sub-rotinas com variáveis de escopo local.

---

## Pontos-chave

- **Parâmetro vs. argumento:** parâmetro = valor *esperado* pela sub-rotina (na declaração); argumento = valor *passado* pelo chamador na execução.
- **Passagem por valor:** uma cópia do dado é enviada; alterações dentro da sub-rotina não afetam a variável original. Útil quando a sub-rotina apenas calcula com os dados recebidos.
  ```
  PROCEDIMENTO CALCULA (INTEIRO: V1, V2, V3)
    DECLARE INTEIRO: SOMA;
    SOMA <- V1 + V2 + V3;
    ESCREVA ("RESULTADO = ", SOMA);
  FIM;
  ```
- **Passagem por referência:** a palavra reservada `VAR` indica que a referência (endereço) ao dado original é passada; toda modificação no parâmetro altera diretamente a variável da origem.
  ```
  PROCEDIMENTO CALCULA (INTEIRO: V1, V2, V3, VAR INTEIRO: SOMA)
    SOMA <- V1 + V2 + V3;
  FIM;
  ```
- **Economia de memória:** por referência evita cópia de dados grandes (ex.: vetores/registros), reduzindo uso de memória — relevante para dispositivos com recursos limitados.
- **Quando usar cada tipo:**
  - Por valor: quando não se quer que a sub-rotina altere os originais.
  - Por referência: quando se quer que a sub-rotina produza resultado em variável externa (alternativa ao retorno de função).

---

## Conceitos relacionados

- [Sub-Rotinas](../conceitos/sub-rotinas.md)
- [Passagem de Parâmetros](../conceitos/passagem-de-parametros.md)
- [Escopo](../conceitos/escopo.md)
- [Ponteiros](../conceitos/ponteiros.md)

---

## Perguntas abertas

- Em Java, primitivos são passados por valor e objetos por referência — como isso se reflete nos conceitos desta aula?
- Qual a relação entre passagem por referência e ponteiros em C?
