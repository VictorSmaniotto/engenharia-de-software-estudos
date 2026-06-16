---
titulo: "ALP A05 — Tipos de Dados"
tipo: fonte
tags: [tipos-de-dados, variaveis, atribuicao, declaracao, algoritmo]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a05-tipos-de-dados]
criado: 2026-05-28
atualizado: 2026-05-28
---

# ALP A05 — Tipos de Dados

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Algoritmos e Lógica de Programação |
| Aula | 05 |
| Ingerida em | 2026-05-28 |

---

## Resumo

A aula apresenta os quatro tipos básicos de dados em algoritmos, a declaração e uso de variáveis como estruturas temporárias de armazenamento em memória, o operador de atribuição `<-` e a estrutura básica de um algoritmo completo (INÍCIO / DECLARE / FIM).

---

## Pontos-chave

### Tipos Básicos de Dados

| Tipo | Descrição | Exemplo de valor |
|------|-----------|-----------------|
| `INTEIRO` | Números sem casas decimais | `20`, `-5` |
| `REAL` | Números com casas decimais | `50.5`, `3.14` |
| `CARACTERE` | Caractere simples ou cadeia de caracteres (string) | `"RONIE"`, `'A'` |
| `LÓGICO` | Apenas verdadeiro ou falso | `VERDADEIRO`, `FALSO` |

### Variáveis

- Estruturas de armazenamento temporário em memória, cujo valor pode mudar durante a execução
- Dados são perdidos ao fim da execução (volatilidade alta)
- Declaração segundo Forbellone (2005): `TIPO: NOME_VARIAVEL;`
- Separador `,` permite declarar múltiplas variáveis do mesmo tipo em uma linha

Exemplos:
```
INTEIRO: IDADE
REAL: PESO, ALTURA
CARACTERE: LETRA
LÓGICO: TESTE
```

- Variável sem tipo definido recebe o tipo do primeiro dado inserido — reduz previsibilidade e aumenta risco de erros

### Atribuição de Dados

- Operador `<-`: dado ou resultado de expressão à direita é armazenado na variável à esquerda
- Expressões são calculadas **antes** da atribuição

```
IDADE <- 20
PESO <- 50.5
NOME <- "RONIE"
MEDIA <- (VALOR1 + VALOR2) / 2
```

- Boa prática: **inicializar variáveis** antes do primeiro uso para evitar valores indesejados em memória

### Estrutura Básica de Algoritmo

Padrão adotado pelo material (unindo Forbellone 2005, Manzano 1997 e Ascencio 2012):

```
INÍCIO
DECLARE
  INTEIRO A, B, C;
  A <- 10;
  B <- A * 2;
  C <- A * B;
FIM.
```

- `INÍCIO` — primeira instrução
- `DECLARE` — seção de declaração de variáveis
- `FIM.` — encerra o algoritmo
- `;` encerra cada instrução (quebras de linha não encerram instrução)
- Letras maiúsculas por convenção do material (destaque visual)

---

## Conexões com o que já existe na wiki

- [Tipos de Dados](../conceitos/tipos-de-dados.md) — conceito central desta aula
- [Variáveis e Constantes](../conceitos/variaveis-e-constantes.md) — conceito central desta aula
- [Pseudocódigo](../conceitos/pseudocodigo.md) — estrutura INÍCIO/DECLARE/FIM é parte do pseudocódigo
- [Palavras Reservadas](../conceitos/palavras-reservadas.md) — INÍCIO, DECLARE, FIM, INTEIRO, REAL, CARACTERE, LÓGICO são palavras reservadas
- [Operadores e Expressões](../conceitos/operadores-e-expressoes.md) — atribuição `<-` e expressões são usadas nesta aula

## Autores Referenciados

- [Forbellone (2005)](../autores/forbellone.md) — sintaxe de declaração de variáveis
- [Manzano (1997)](../autores/manzano.md) — sintaxe de algoritmos
- [Ascencio (2012)](../autores/ascencio.md) — sintaxe adotada neste material (poucos símbolos)
