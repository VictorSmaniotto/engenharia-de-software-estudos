---
titulo: "ALP A07 — Estruturas de Decisão"
tipo: fonte
tags: [estruturas-de-decisao, condicional, se-entao, senao, escolha-caso, fluxo-de-execucao]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a07-estruturas-de-decisao]
criado: 2026-05-28
atualizado: 2026-05-28
---

# ALP A07 — Estruturas de Decisão

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Algoritmos e Lógica de Programação |
| Aula | 07 |
| Ingerida em | 2026-05-28 |

---

## Resumo

A aula apresenta as estruturas de controle de fluxo baseadas em decisão: simples (`SE...ENTÃO...FIMSE`), composta (`SE...ENTÃO...SENÃO...FIMSE`), aninhada (múltiplas condições encadeadas) e de seleção múltipla (`ESCOLHA...CASO...FIMESCOLHA`).

---

## Pontos-chave

### Estruturas de Controle

- Definem critérios para que instruções ou blocos sejam executados **condicionalmente**
- Sem elas, algoritmos executam apenas de forma sequencial
- A condição utiliza operadores relacionais e lógicos (vistos na A04)

### 1. Decisão Simples — `SE...ENTÃO...FIMSE`

Executa um bloco apenas se a condição for verdadeira.

```
SE (VALOR >= 0) ENTÃO
  ESCREVA ("NÚMERO POSITIVO");
FIMSE;
```

### 2. Decisão Composta — `SE...ENTÃO...SENÃO...FIMSE`

Executa um bloco se verdadeiro, outro se falso.

```
SE (VALOR >= 0) ENTÃO
  ESCREVA ("NÚMERO POSITIVO");
SENÃO
  ESCREVA ("NÚMERO NEGATIVO");
FIMSE;
```

### 3. Decisão Aninhada

**Forma 1 — múltiplas opções encadeadas** (`SENÃO SE`):

```
SE (OPCAO = 1) ENTÃO
  ESCREVA ("PRIMEIRA");
SENÃO SE (OPCAO = 2) ENTÃO
  ESCREVA ("SEGUNDA");
SENÃO SE (OPCAO = 3) ENTÃO
  ESCREVA ("TERCEIRA");
SENÃO SE (OPCAO = 4) ENTÃO
  ESCREVA ("QUARTA");
SENÃO
  ESCREVA ("OPÇÃO DESCONHECIDA");
FIMSE; FIMSE; FIMSE; FIMSE;
```

**Forma 2 — condições complementares** (segunda condição só avaliada se a primeira for verdadeira):

```
SE (DOCUMENTO = VERDADEIRO) ENTÃO
  SE (IDADE >= 18) ENTÃO
    ESCREVA ("ENTRADA PERMITIDA");
  SENÃO
    ESCREVA ("MENOR DE IDADE");
SENÃO
  ESCREVA ("SEM DOCUMENTO");
FIMSE;
```

- Recomenda-se **indentação** crescente a cada nível de aninhamento para legibilidade

### 4. Seleção Múltipla — `ESCOLHA...CASO...FIMESCOLHA`

Alternativa mais legível ao `SE` aninhado para múltiplos valores discretos de **uma única variável**:

```
ESCOLHA OPCAO
  CASO 1: ESCREVA ("PRIMEIRA");
  CASO 2: ESCREVA ("SEGUNDA");
  CASO 3: ESCREVA ("TERCEIRA");
  CASO 4: ESCREVA ("QUARTA");
  CASO CONTRÁRIO: ESCREVA ("OPÇÃO DESCONHECIDA");
FIMESCOLHA;
```

**Limitação**: aceita apenas comparação de **igualdade** com valores discretos de uma variável — não suporta expressões relacionais ou lógicas compostas.

---

## Conexões com o que já existe na wiki

- [Estruturas de Decisão](../conceitos/estruturas-de-decisao.md) — conceito central desta aula
- [Operadores e Expressões](../conceitos/operadores-e-expressoes.md) — condições usam operadores relacionais e lógicos
- [Palavras Reservadas](../conceitos/palavras-reservadas.md) — SE, ENTÃO, SENÃO, FIMSE, ESCOLHA, CASO, FIMESCOLHA
- [Entrada e Saída de Dados](../conceitos/entrada-e-saida-de-dados.md) — validação de entradas usa estruturas de decisão
