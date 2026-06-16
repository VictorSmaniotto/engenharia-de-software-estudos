---
titulo: Variáveis e Constantes
tipo: conceito
tags: [variaveis, constantes, atribuicao, declaracao, memoria, algoritmo]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a05-tipos-de-dados]
criado: 2026-05-28
atualizado: 2026-05-28
---

# Variáveis e Constantes

## Definição

**Variáveis** são estruturas de armazenamento temporário em memória associadas a um tipo de dado. Seu valor pode ser alterado livremente durante a execução do algoritmo. Os dados são perdidos ao final da execução (volatilidade alta).

**Constantes** complementam as variáveis como recurso de armazenamento cujo valor **não muda** durante a execução do algoritmo.

---

## Declaração de Variáveis

Sintaxe segundo Forbellone (2005):

```
TIPO: NOME_VARIAVEL;
```

Múltiplas variáveis do mesmo tipo:

```
REAL: PESO, ALTURA;
```

Exemplos:

```
INTEIRO: IDADE
REAL: PESO, ALTURA
CARACTERE: LETRA
LÓGICO: TESTE
```

- Declarações ficam na seção `DECLARE`, antes das instruções do algoritmo
- `;` encerra cada instrução
- `,` separa múltiplas variáveis na mesma declaração

---

## Atribuição de Dados

O operador `<-` armazena um valor ou resultado de expressão em uma variável:

```
IDADE <- 20
PESO <- 50.5
NOME <- "RONIE"
MEDIA <- (VALOR1 + VALOR2) / 2
```

- O lado direito é **sempre avaliado antes** da atribuição
- Boa prática: **inicializar** variáveis antes do primeiro uso para evitar valores residuais em memória

---

## Estrutura Básica de Algoritmo

```
INÍCIO
DECLARE
  INTEIRO A, B, C;
  A <- 10;
  B <- A * 2;
  C <- A * B;
FIM.
```

- `INÍCIO` abre o algoritmo
- `DECLARE` delimita a seção de declarações
- `FIM.` encerra o algoritmo

---

## Relações

- [Tipos de Dados](tipos-de-dados.md) — toda variável está associada a um tipo
- [Operadores e Expressões](operadores-e-expressoes.md) — expressões são atribuídas a variáveis
- [Pseudocódigo](pseudocodigo.md) — variáveis e atribuição são elementos centrais do pseudocódigo
- [Palavras Reservadas](palavras-reservadas.md) — INÍCIO, DECLARE, FIM são palavras reservadas
- [Escopo](escopo.md) — variáveis locais têm ciclo de vida limitado ao bloco/função

## Fontes

- [ALP A05 — Tipos de Dados](../fontes/alp-a05-tipos-de-dados.md)
- [Forbellone (2005)](../autores/forbellone.md)
- [Manzano (1997)](../autores/manzano.md)
- [Ascencio (2012)](../autores/ascencio.md)
