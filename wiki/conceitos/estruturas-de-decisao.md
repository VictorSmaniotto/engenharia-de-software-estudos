---
titulo: Estruturas de Decisão
tipo: conceito
tags: [estruturas-de-decisao, condicional, se-entao, senao, fimse, escolha-caso, fluxo-de-execucao]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a07-estruturas-de-decisao]
criado: 2026-05-28
atualizado: 2026-05-28
---

# Estruturas de Decisão

## Definição

Estruturas de decisão são mecanismos de **controle de fluxo** que permitem executar instruções condicionalmente, com base no resultado (verdadeiro/falso) de uma expressão condicional. Sem elas, algoritmos executam apenas sequencialmente.

---

## Tipos

### 1. Decisão Simples — `SE...ENTÃO...FIMSE`

Executa um bloco **apenas se** a condição for verdadeira; não há alternativa para o caso falso.

```
SE (VALOR >= 0) ENTÃO
  ESCREVA ("NÚMERO POSITIVO");
FIMSE;
```

### 2. Decisão Composta — `SE...ENTÃO...SENÃO...FIMSE`

Executa um bloco para verdadeiro e **outro bloco** para falso.

```
SE (VALOR >= 0) ENTÃO
  ESCREVA ("NÚMERO POSITIVO");
SENÃO
  ESCREVA ("NÚMERO NEGATIVO");
FIMSE;
```

### 3. Decisão Aninhada

**Múltiplas opções encadeadas** — cada `SENÃO` contém uma nova estrutura `SE`:

```
SE (OPCAO = 1) ENTÃO
  ESCREVA ("PRIMEIRA");
SENÃO SE (OPCAO = 2) ENTÃO
  ESCREVA ("SEGUNDA");
SENÃO SE (OPCAO = 3) ENTÃO
  ESCREVA ("TERCEIRA");
SENÃO
  ESCREVA ("DESCONHECIDA");
FIMSE; FIMSE; FIMSE;
```

**Condições complementares** — segunda condição só avaliada se a primeira for verdadeira:

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

- Usar **indentação** crescente a cada nível para legibilidade

### 4. Seleção Múltipla — `ESCOLHA...CASO...FIMESCOLHA`

Alternativa mais compacta e legível para múltiplos valores discretos de uma única variável.

```
ESCOLHA OPCAO
  CASO 1: ESCREVA ("PRIMEIRA");
  CASO 2: ESCREVA ("SEGUNDA");
  CASO 3: ESCREVA ("TERCEIRA");
  CASO CONTRÁRIO: ESCREVA ("DESCONHECIDA");
FIMESCOLHA;
```

**Limitação**: suporta apenas igualdade de valor com uma variável — não aceita expressões lógicas ou relacionais compostas.

---

## Comparativo

| Estrutura | Alternativas | Aceita expressão lógica? | Melhor uso |
|-----------|-------------|--------------------------|-----------|
| `SE` simples | 1 (verdadeiro) | Sim | Execução opcional |
| `SE...SENÃO` | 2 | Sim | Bifurcação binária |
| `SE` aninhado | N | Sim | Múltiplas condições complexas |
| `ESCOLHA...CASO` | N | Não | Múltiplos valores discretos de 1 variável |

---

## Relações

- [Operadores e Expressões](operadores-e-expressoes.md) — condições usam operadores relacionais e lógicos
- [Estruturas de Repetição](estruturas-de-repeticao.md) — podem ser aninhadas dentro de laços
- [Entrada e Saída de Dados](entrada-e-saida-de-dados.md) — validação de entradas usa condicionais
- [Palavras Reservadas](palavras-reservadas.md) — SE, ENTÃO, SENÃO, FIMSE, ESCOLHA, CASO, FIMESCOLHA

## Fontes

- [ALP A07 — Estruturas de Decisão](../fontes/alp-a07-estruturas-de-decisao.md)
