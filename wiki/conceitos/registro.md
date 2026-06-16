---
titulo: Registro (Estrutura Heterogênea)
tipo: conceito
tags: [registro, struct, heterogeneo, campos, banco-de-dados]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula12-estruturas-heterogeneas, alp-aula16-manipulacao-arquivos]
criado: 2026-06-15
atualizado: 2026-06-15
---

# Registro (Estrutura Heterogênea)

## Definição

Um **registro** é uma estrutura de dados que agrupa campos de **tipos diferentes** sob um único identificador. Contrasta com estruturas homogêneas ([vetores e matrizes](vetores-e-matrizes.md)), onde todos os elementos têm o mesmo tipo.

Em algumas linguagens, o mesmo conceito é chamado de `struct` (C) ou `record` (Pascal).

## Declaração (sintaxe Forbellone)

```
TIPO CADASTRO = REGISTRO
  INTEIRO: CODIGO, IDADE;
  CARACTERE: NOME, ENDERECO, CIDADE, ESTADO
FIMREGISTRO;

CADASTRO: DADOS;
```

A palavra `TIPO` define o registro como um novo tipo de dado; `DADOS` é a variável concreta do tipo `CADASTRO`.

## Acesso a Campos

Notação com ponto: `DADOS.CODIGO`, `DADOS.NOME`. Cada campo é acessado individualmente, diferente do índice numérico dos vetores.

```
LEIA (DADOS.CODIGO);
LEIA (DADOS.NOME);
ESCREVA ("NOME: ", DADOS.NOME);
```

## Conexão com Bancos de Dados

A estrutura de um registro em algoritmos é análoga a uma linha (tupla) de uma tabela relacional: cada campo corresponde a uma coluna. A aula menciona essa relação explicitamente, indicando que os conceitos de algoritmos e bancos de dados se cruzam neste ponto.

## Combinação com Vetores

É possível declarar um vetor de registros:
```
TIPO DADOS = VETOR [1..100] DE CADASTRO;
```
Isso cria uma estrutura equivalente a uma tabela em memória — 100 linhas, cada uma com os campos do registro `CADASTRO`.

## Uso em Arquivos

Registros são a base para definir o tipo de um arquivo de dados:
```
TIPO ARQ = ARQUIVO COMPOSTO DE CADASTRO;
```
Ver [Manipulação de Arquivos](manipulacao-de-arquivos.md).

## Relações

- [Vetores e Matrizes](vetores-e-matrizes.md)
- [Manipulação de Arquivos](manipulacao-de-arquivos.md)
- [Tipos de Dados](tipos-de-dados.md)
- [Ponteiros](ponteiros.md) — em C, `struct` é acessada frequentemente via ponteiro
