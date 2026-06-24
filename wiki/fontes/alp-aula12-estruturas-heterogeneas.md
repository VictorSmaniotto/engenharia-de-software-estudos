---
titulo: "ALP Aula 12 — Estruturas de Dados Heterogêneas (Registros)"
tipo: fonte
tags: [registro, estrutura-heterogenea, campos, banco-de-dados]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-aula12-estruturas-heterogeneas]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 12 — Estruturas de Dados Heterogêneas (Registros)

**Disciplina:** Algoritmos e Lógica de Programação  
**Módulo/Aula:** Aula 12  
**Data de ingestão:** 2026-06-15

---

## Resumo

Apresenta as **estruturas de dados heterogêneas** (registros), que permitem agrupar campos de diferentes tipos sob um único identificador — ao contrário das estruturas homogêneas (vetores/matrizes), onde todos os elementos são do mesmo tipo.

---

## Pontos-chave

- **Registro:** estrutura que contém campos de tipos diferentes. Em algumas linguagens chamado de `struct`.
- **Declaração (sintaxe Forbellone):**
  ```
  TIPO CADASTRO = REGISTRO
    INTEIRO: CODIGO, IDADE;
    CARACTERE: NOME, ENDERECO, CIDADE, ESTADO
  FIMREGISTRO;
  CADASTRO: DADOS;
  ```
  O tipo `CADASTRO` é definido pelo desenvolvedor e usado como tipo em declarações de variáveis.
- **Acesso a campos:** notação com ponto — `DADOS.CODIGO`, `DADOS.NOME`. Difere de vetores onde se usa índice numérico.
- **Conexão com bancos de dados:** conceitos de registro em algoritmos se aproximam da teoria de tabelas relacionais (linha = registro, coluna = campo).
- **Combinação com vetores:** é possível declarar um vetor cujo tipo base é um registro, criando uma lista de registros — estrutura equivalente a uma tabela de banco de dados em memória.

---

## Conceitos relacionados

- [Registro](../conceitos/registro.md)
- [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md)
- [Tipos de Dados](../conceitos/tipos-de-dados.md)

---

## Perguntas abertas

- Como a estrutura `REGISTRO` em algoritmos se mapeia para `struct` em C e objetos em Java?
- Qual a diferença prática entre usar um registro e usar variáveis separadas para cada campo?
