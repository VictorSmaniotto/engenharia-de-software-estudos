---
titulo: "LP A4 — Programação Estruturada: Linguagem C"
tipo: fonte
tags: [linguagem-c, programacao-estruturada, ponteiros, vetores, matrizes, escopo, funcoes]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-11
atualizado: 2026-05-11
---

# LP A4 — Programação Estruturada: Linguagem C

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Linguagens de Programação |
| Aula | 4 |
| Título original | Aula 04 - Programação Estruturada - Linguagem C |
| Fonte original | https://ead.unimar.br/aulas/linguagens-de-programacao/aula-04.html |
| Data de ingestão | 2026-05-11 |

---

## Resumo

Apresenta a linguagem C como exemplo ideal para o estudo da programação estruturada. Detalha sua estrutura baseada em funções, sintaxe com delimitadores, estruturas de controle (if/else, while), indentação, e conceitos avançados como ponteiros, escopo de variáveis, e estruturas de dados homogêneas (vetores e matrizes).

---

## Pontos-chave

### Linguagem C — Visão Geral
- Exemplo mais apropriado para estudo da programação estruturada pela riqueza de funcionalidades
- Cobre desde baixo nível até alto nível
- Filhas: **C++** (computação gráfica), **C#** (desenvolvimento web/desktop), **Objective-C** (iOS)
- Muitas linguagens modernas (Java, JavaScript) herdaram sintaxe e delimitadores do C

### Funções e main()
- A base da linguagem C são **funções**: blocos independentes de código que trocam dados entre si por parâmetros
- Todo software em C tem exatamente uma função `main()` — ponto de entrada da execução
- `main()` é nome reservado; nenhuma outra função pode ter este nome no mesmo software

### Sintaxe e Delimitadores
- Linguagem **case sensitive**: maiúsculas e minúsculas tratadas como diferentes; palavras reservadas em minúsculas
- **`;`** — encerra comandos
- **`{ }`** — delimita blocos de comandos dentro de estruturas de controle
- **`( )`** — delimita parâmetros de funções e condições de comandos (if, while)
- **`[ ]`** — delimita índices de vetores e matrizes

### Estruturas de Controle
- **`if / else`**: desvio condicional com expressão lógica entre parênteses
- **`while`**: laço de repetição controlado por condição; executa enquanto a condição for verdadeira
- **Aninhamento**: estruturas do mesmo tipo ou diferentes podem ser encadeadas (ex.: if dentro de if, while dentro de while)
- **Indentação/endentação**: não obrigatória na linguagem, mas essencial para legibilidade

### Escopo de Variáveis
- Variáveis declaradas **dentro de uma função** existem apenas enquanto a função é executada
- Ao entrar na função: espaço alocado em memória; ao sair: espaço liberado
- Consequência: alterar `a` e `b` dentro de uma função não afeta as variáveis originais (passagem por valor)

### Ponteiros
- Estrutura que armazena um **endereço de memória**, não um valor em si
- Sintaxe: `*` para declarar ponteiro e acessar o valor apontado; `&` para obter o endereço de uma variável
- Permite que alterações dentro de uma função afetem variáveis fora dela (passagem por referência)
- Necessário quando se quer retornar mais de um valor de uma função (C retorna apenas um valor por padrão)
- Exemplo: função `trocaValores(*a, *b)` com ponteiros altera os valores originais; sem ponteiros, não

### Vetores e Matrizes
- Estruturas de dados **homogêneas** (todos os elementos do mesmo tipo)
- **Vetor**: 1 dimensão — `int lista[10];` (10 inteiros, índices 0 a 9)
- **Matriz**: 2+ dimensões — `char dados[3][9];` (3 linhas × 9 colunas = 27 caracteres)
- Índices iniciam em **zero** por convenção da linguagem C
- Referência via colchetes: `lista[2]`, `dados[1][4]`
- Vetores e matrizes são naturalmente manipulados com estruturas de repetição

### Bibliotecas
- `#include <stdio.h>` — inclui a biblioteca padrão de entrada/saída
- Disponibiliza funções `printf()` (saída) e `scanf()` (entrada)

---

## Conexões com o que já existe na wiki

- Concretiza [Paradigma Estruturado](../conceitos/paradigma-estruturado.md) com exemplo real em C
- Cria base para [Linguagem C](../conceitos/linguagem-c.md)
- Cria base para [Ponteiros](../conceitos/ponteiros.md)
- Cria base para [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md)
- Cria base para [Escopo](../conceitos/escopo.md)
- Aprofunda [Sintaxe e Semântica](../conceitos/sintaxe-e-semantica.md) com exemplos práticos em C

---

## Perguntas abertas

- Quando se deve usar ponteiros vs retorno de função vs variáveis globais para compartilhar dados entre funções?
- Como alocação dinâmica de memória (`malloc`) se relaciona com o conceito de escopo?
