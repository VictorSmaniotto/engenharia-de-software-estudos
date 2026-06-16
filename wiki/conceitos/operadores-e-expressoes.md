---
titulo: Operadores e Expressões
tipo: conceito
tags: [operadores, expressoes, logica, precedencia, tabela-verdade, algoritmo]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a04-operadores-e-expressoes]
criado: 2026-05-28
atualizado: 2026-05-28
---

# Operadores e Expressões

## Definição

Operadores são símbolos com finalidades específicas que permitem realizar cálculos, comparações e combinações lógicas em algoritmos. Expressões são combinações de valores, variáveis e operadores que resultam em um valor.

---

## Tipos de Operadores

### Matemáticos

| Operador | Descrição |
|----------|-----------|
| `+` | Soma |
| `-` | Subtração |
| `*` | Multiplicação |
| `/` | Divisão |
| `%` | Resto da divisão inteira (módulo) |

Os símbolos `*` e `/` substituem `×` e `÷` por limitações do teclado.

### Relacionais

Comparam dois valores e retornam **verdadeiro** ou **falso**:

| Operador | Descrição |
|----------|-----------|
| `>` | Maior |
| `>=` | Maior ou igual |
| `<` | Menor |
| `<=` | Menor ou igual |
| `=` | Igual |
| `<>` | Diferente |

### Lógicos

Combinam expressões relacionais em comparações compostas; também retornam verdadeiro ou falso:

| Operador | Comportamento |
|----------|--------------|
| **E** | Verdadeiro somente se **todas** as expressões forem verdadeiras |
| **OU** | Verdadeiro se **pelo menos uma** expressão for verdadeira |
| **NÃO** | Inverte o valor lógico da expressão |

Outros operadores lógicos existentes: NOR, NAND, XOR (não detalhados na disciplina).

---

## Precedência de Operadores

Ordem de avaliação (da maior para menor prioridade):

1. `( )` — parênteses (mais internos primeiro)
2. `*` `/` `%` — multiplicação, divisão, módulo
3. `+` `-` — soma, subtração
4. `>` `>=` `<` `<=` `=` `<>` — relacionais (mesmo nível entre si)
5. `E` `OU` `NÃO` — lógicos

Parênteses anulam a precedência natural: `5 + (3 * 2 - (1 + 4))` avalia `(1+4)=5` primeiro, depois `3*2=6`, depois `6-5=1`, e por fim `5+1=6`.

---

## Expressões em Algoritmos

- **Matemáticas**: usadas em atribuições para calcular e armazenar resultados em variáveis
- **Relacionais/lógicas**: usadas principalmente em condições de estruturas de controle (`SE ... ENTÃO`, laços de repetição)

```
SOMA <- 3 + 5
MEDIA <- (VALOR1 + VALOR2) / 2
SE (IDADE >= 18) ENTÃO
SE (VALOR > 0 E VALOR < 10) ENTÃO
```

---

## Relações

- [Variáveis e Constantes](variaveis-e-constantes.md) — variáveis recebem resultados de expressões via atribuição `<-`
- [Pseudocódigo](pseudocodigo.md) — operadores e expressões fazem parte da sintaxe do pseudocódigo
- [Palavras Reservadas](palavras-reservadas.md) — `SE`, `ENTÃO` são palavras reservadas usadas com expressões lógicas
- [Tipos de Dados](tipos-de-dados.md) — o tipo do resultado de uma expressão depende dos tipos dos operandos

## Fontes

- [ALP A04 — Operadores e Expressões](../fontes/alp-a04-operadores-e-expressoes.md)
