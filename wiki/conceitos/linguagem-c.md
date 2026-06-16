---
titulo: Linguagem C
tipo: conceito
tags: [linguagem-c, programacao-estruturada, funcoes, ponteiros, compilada]
disciplina: Linguagens de Programação
fontes: [lp-a04-programacao-estruturada-linguagem-c]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Linguagem C

## Definição

Linguagem de programação compilada, de propósito geral, considerada o exemplo mais representativo do [Paradigma Estruturado](paradigma-estruturado.md). Cobre desde operações de baixo nível (manipulação de memória, ponteiros) até alto nível (estruturas de dados complexas, bibliotecas).

## Características Principais

| Característica | Detalhe |
|---------------|---------|
| Paradigma base | Estruturado (funções independentes) |
| Case sensitive | `Main` ≠ `main` ≠ `MAIN`; palavras reservadas em minúsculas |
| Ponto de entrada | `main()` — obrigatória e única |
| Compilação | Gera executável nativo (baixa portabilidade entre plataformas) |

## Sintaxe e Delimitadores

- **`;`** — encerra cada instrução
- **`{ }`** — delimita blocos de comandos (funções, if, while)
- **`( )`** — delimita parâmetros de funções e condições de controle
- **`[ ]`** — delimita índices de vetores e matrizes

Esses delimitadores foram adotados por muitas linguagens posteriores (Java, JavaScript, C#).

## Estrutura Básica

```c
#include <stdio.h>   // biblioteca padrão de E/S

int main() {
    // ponto de entrada; toda execução começa aqui
    return 0;
}
```

## Estruturas de Controle

- **`if / else`**: desvio condicional com expressão lógica
- **`while`**: laço de repetição por condição
- Aninhamento de estruturas é amplamente utilizado para algoritmos mais complexos

## Conceitos Avançados

- **[Ponteiros](ponteiros.md)**: armazenam endereços de memória; permitem passagem por referência
- **[Vetores e Matrizes](vetores-e-matrizes.md)**: estruturas de dados homogêneas indexadas
- **[Escopo](escopo.md)**: variáveis de uma função existem apenas durante sua execução
- **[Bibliotecas](../conceitos/compilacao-e-interpretacao.md)**: código externo incluído via `#include`

## Família C

| Linguagem | Foco |
|-----------|------|
| **C++** | Orientação a objetos, computação gráfica |
| **C#** | Desenvolvimento web/desktop (Microsoft) |
| **Objective-C** | Plataforma Apple/iOS |

## Relações

- [Paradigma Estruturado](paradigma-estruturado.md) — linguagem canônica deste paradigma
- [Compilação e Interpretação](compilacao-e-interpretacao.md) — C é compilada classicamente
- [Sintaxe e Semântica](sintaxe-e-semantica.md) — C tem sintaxe explícita e rigorosa

## Fontes

- [LP A4 — Programação Estruturada: Linguagem C](../fontes/lp-a04-programacao-estruturada-linguagem-c.md)
