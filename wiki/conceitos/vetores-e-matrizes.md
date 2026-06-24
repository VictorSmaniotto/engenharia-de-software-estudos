---
titulo: Vetores e Matrizes
tipo: conceito
tags: [vetores, matrizes, estruturas-de-dados, linguagem-c, arrays, homogeneas]
disciplina: Algoritmos e Lógica de Programação
fontes: [lp-a04-programacao-estruturada-linguagem-c, alp-aula10-estruturas-homogeneas, alp-aula11-estruturas-homogeneas-multidimensionais]
criado: 2026-05-11
atualizado: 2026-06-15
---

# Vetores e Matrizes

## Definição

Estruturas de dados **homogêneas**: conjuntos de elementos do mesmo tipo acessados por índices numéricos.

| Estrutura | Dimensões | Exemplo |
|-----------|-----------|---------|
| **Vetor** | 1 (lista linear) | `int lista[10]` |
| **Matriz** | 2+ (linhas × colunas) | `char dados[3][9]` |

> Alguns autores usam "matriz" para qualquer quantidade de dimensões; outros reservam "vetor" para 1D. (LP A4)

## Sintaxe em C

```c
int lista[10];         // vetor: 10 inteiros (índices 0 a 9)
char dados[3][9];      // matriz: 3 linhas × 9 colunas = 27 chars
```

- Índices iniciam em **zero** por convenção da linguagem C
- Acesso: `lista[2]` (terceiro elemento), `dados[1][4]` (linha 1, coluna 4)
- Delimitados por **colchetes** `[ ]`

## Relação com Estruturas de Repetição

Vetores e matrizes são naturalmente processados com laços (`while`, `for`):
- Um contador funciona como índice do vetor
- Dois contadores encadeados percorrem linhas e colunas de uma matriz (como ponteiros de um relógio ou dígitos de um hodômetro)

## Sintaxe em Portugol/Pseudocódigo (ALP)

```
TIPO DADOS = VETOR [1..10] DE INTEIROS;
DADOS: LISTA;
```

Acesso por índice: `LISTA[I]`. Índices iniciam em 1 por convenção no Portugol (diferente de C onde iniciam em 0).

### Matrizes em Portugol

```
TIPO TABULEIRO = MATRIZ [1..8][1..8] DE CARACTERES;
TIPO VELHA     = MATRIZ [1..3][1..3] DE CARACTERES;
TIPO CUBOMAGICO = MATRIZ [1..3][1..3][1..3] DE INTEIRO;
```

Acesso 2D: `VELHA[I,J]` (VisualG usa vírgula) ou `VELHA[I][J]`.

### Aplicações práticas de matrizes
- **Imagens:** cada pixel é uma célula com valor de cor (ex.: 1024×768 pixels → matriz 1024×768).
- **Jogos de tabuleiro:** xadrez, damas, jogo da velha — posição de peças em linha×coluna.
- **Space Invaders e similares:** posição de elementos na tela representada como coordenadas matriciais.

## Busca em Vetores

Dois padrões:
1. `PARA I DE 1 ATÉ N` — percorre todo o vetor (mais simples, menos eficiente).
2. `ENQUANTO (LISTA[I] <> BUSCA OU I <= N)` — interrompe ao encontrar o valor.

## Relações

- [Linguagem C](linguagem-c.md) — sintaxe de declaração e acesso em C
- [Ponteiros](ponteiros.md) — ponteiros são frequentemente usados para manipular vetores/matrizes em C
- [Aninhamento de Estruturas](aninhamento-de-estruturas.md) — percorrer matrizes 2D requer laços aninhados
- [Registro](registro.md) — vetor de registros = lista de estruturas heterogêneas em memória

## Fontes

- [LP A4 — Programação Estruturada: Linguagem C](../fontes/lp-a04-programacao-estruturada-linguagem-c.md)
- [ALP Aula 10 — Estruturas Homogêneas (Vetores)](../fontes/alp-aula10-estruturas-homogeneas.md)
- [ALP Aula 11 — Estruturas Homogêneas Multidimensionais (Matrizes)](../fontes/alp-aula11-estruturas-homogeneas-multidimensionais.md)
