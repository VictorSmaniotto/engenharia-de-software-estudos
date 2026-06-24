---
titulo: Pseudocódigo
tipo: conceito
tags: [algoritmo, pseudocodigo, portugol, representacao]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a01-conceitos-gerais-de-programacao]
criado: 2026-05-07
atualizado: 2026-05-07
---

# Pseudocódigo

## Definição

Forma de representar algoritmos usando uma linguagem próxima das linguagens de programação, mas ainda legível em idioma local. No Brasil, a variante é chamada de **Portugol**. Usa palavras reservadas padronizadas e tem maior nível de detalhamento que a descrição narrativa.

> "Representações em idioma local de uma possível solução computacional, mais visando a compreensão lógica de uma solução proposta." (ALP A1)

Não é executável diretamente — precisa ser convertido em uma linguagem de programação real.

## Estrutura básica

```
INÍCIO
  DECLARE
    INTEIRO: VALOR;
  LEIA (VALOR);
  SE (VALOR >= 0)
    ENTÃO ESCREVA ("VALOR POSITIVO");
    SENÃO ESCREVA ("VALOR NEGATIVO");
  FIMSE;
FIM.
```

## Variações de padronização

A sintaxe varia entre autores. O material da disciplina segue **Forbellone** (com extensões de **Manzano**). Diferenças comuns: símbolos usados, nomes das palavras reservadas.

## Comparação com outras formas de representação

| Forma | Nível de detalhe | Proximidade com código |
|-------|-----------------|----------------------|
| Descrição narrativa | Baixo | Baixa |
| [Fluxograma](fluxograma.md) | Médio | Baixa |
| **Pseudocódigo** | Alto | Alta |

## Relações

- [Fluxograma](fluxograma.md) — representação alternativa do mesmo algoritmo
- [Palavras Reservadas](palavras-reservadas.md)

## Fontes

- [ALP A1 — Conceitos Gerais de Programação](../fontes/alp-a01-conceitos-gerais-de-programacao.md)
