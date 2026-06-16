---
titulo: Ponteiros
tipo: conceito
tags: [ponteiros, memoria, linguagem-c, passagem-por-referencia]
disciplina: Linguagens de Programação
fontes: [lp-a04-programacao-estruturada-linguagem-c]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Ponteiros

## Definição

Estrutura de dados que armazena um **endereço de memória** (e não um valor em si). Ao apontar para a posição de outra variável, permite acessar e modificar o valor dessa variável de qualquer parte do código, inclusive de dentro de funções.

> "Ponteiros servem como indicativos de outra estrutura de dados em memória e não armazenam dados em si." (LP A4)

## Sintaxe em C

```c
int x = 10;
int *p = &x;   // p aponta para o endereço de x
*p = 20;       // altera o valor de x via ponteiro (x passa a ser 20)
```

| Símbolo | Significado |
|---------|-------------|
| `*` (na declaração) | Declara uma variável como ponteiro |
| `*` (no uso) | Acessa o valor no endereço apontado (desreferenciação) |
| `&` | Obtém o endereço de memória de uma variável |

## Por que Ponteiros Importam

Em C, parâmetros de função são passados **por valor** (cópia). Alterações internas não afetam as variáveis originais (ver [Escopo](escopo.md)). Ponteiros permitem **passagem por referência**, contornando esta limitação:

```c
// SEM ponteiro: não troca os originais
void trocaValores(int a, int b) { ... }

// COM ponteiro: troca os originais
void trocaValores(int *a, int *b) { ... }
```

C retorna apenas um valor por função; ponteiros são o mecanismo para que uma função modifique múltiplas variáveis externas.

## Relações

- [Escopo](escopo.md) — entender escopo explica por que ponteiros são necessários
- [Linguagem C](linguagem-c.md) — ponteiros são exclusivos/característicos do C (ausentes em Java, por exemplo)
- [Vetores e Matrizes](vetores-e-matrizes.md) — ponteiros são essenciais para manipulação de estruturas de dados maiores

## Fontes

- [LP A4 — Programação Estruturada: Linguagem C](../fontes/lp-a04-programacao-estruturada-linguagem-c.md)
