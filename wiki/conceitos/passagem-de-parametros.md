---
titulo: Passagem de Parâmetros
tipo: conceito
tags: [parametro, argumento, passagem-por-valor, passagem-por-referencia, sub-rotina, var]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula14-parametros]
criado: 2026-06-15
atualizado: 2026-06-15
---

# Passagem de Parâmetros

## Definição

**Parâmetros** são os valores esperados por uma sub-rotina para sua execução. **Argumentos** são os valores efetivamente passados pelo chamador. Parâmetros resolvem o problema de comunicação de dados entre partes de um algoritmo com variáveis de escopo local.

## Passagem por Valor

Uma **cópia** do dado é enviada para a sub-rotina. Alterações internas **não afetam** a variável original.

```
PROCEDIMENTO CALCULA (INTEIRO: V1, V2, V3)
  DECLARE INTEIRO: SOMA;
  SOMA <- V1 + V2 + V3;
  ESCREVA ("RESULTADO = ", SOMA);
FIM;
```

Uso: quando a sub-rotina apenas processa os dados sem precisar modificar as originais.

## Passagem por Referência

A **referência** (endereço) ao dado original é passada via palavra reservada `VAR`. Toda modificação no parâmetro **altera diretamente** a variável de origem.

```
PROCEDIMENTO CALCULA (INTEIRO: V1, V2, V3, VAR INTEIRO: SOMA)
  SOMA <- V1 + V2 + V3;
FIM;
```

Uso: quando se quer que a sub-rotina produza resultado em variável externa sem usar `RETORNE` (alternativa ao retorno de função). Também economiza memória ao não duplicar dados grandes.

## Comparação

| Aspecto | Por Valor | Por Referência |
|---------|-----------|----------------|
| O que é transmitido | Cópia do dado | Endereço do dado |
| Afeta a origem? | Não | Sim |
| Uso típico | Cálculos sem efeito colateral | Produzir resultado em variável externa |
| Memória | Mais uso (cópia) | Menos uso (sem cópia) |

## Parâmetro vs. Argumento

- **Parâmetro:** variável na *declaração* da sub-rotina (`INTEIRO: V1`).
- **Argumento:** valor passado na *chamada* (`CALCULA(A, B, C)`).

## Relações

- [Sub-Rotinas](sub-rotinas.md)
- [Escopo](escopo.md)
- [Ponteiros](ponteiros.md) — passagem por referência é implementada via ponteiros em C
