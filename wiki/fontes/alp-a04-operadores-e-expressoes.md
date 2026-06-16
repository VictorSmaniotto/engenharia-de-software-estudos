---
titulo: "ALP A04 — Operadores e Expressões"
tipo: fonte
tags: [operadores, expressoes, logica, precedencia, tabela-verdade]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a04-operadores-e-expressoes]
criado: 2026-05-28
atualizado: 2026-05-28
---

# ALP A04 — Operadores e Expressões

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Algoritmos e Lógica de Programação |
| Aula | 04 |
| Ingerida em | 2026-05-28 |

---

## Resumo

A aula apresenta os três tipos de operadores utilizados na elaboração de algoritmos — matemáticos, relacionais e lógicos — e explica como são combinados em expressões. Discute a precedência de operadores e o papel dos parênteses na alteração da ordem natural de avaliação.

---

## Pontos-chave

### Operadores Matemáticos

| Operador | Descrição |
|----------|-----------|
| `+` | Soma |
| `-` | Subtração |
| `*` | Multiplicação (substitui ×) |
| `/` | Divisão (substitui ÷) |
| `%` | Resto da divisão inteira (módulo) |

### Operadores Relacionais

Comparam dois dados e retornam **verdadeiro** ou **falso**:

| Operador | Descrição |
|----------|-----------|
| `>` | Maior |
| `>=` | Maior ou igual |
| `<` | Menor |
| `<=` | Menor ou igual |
| `=` | Igual |
| `<>` | Diferente (substitui ≠) |

### Operadores Lógicos

Combinam expressões relacionais em comparações compostas:

| A | B | E | OU |
|---|---|---|----|
| V | V | V | V  |
| V | F | F | V  |
| F | V | F | V  |
| F | F | F | F  |

| A | NÃO A |
|---|-------|
| V | F     |
| F | V     |

- **E**: exige que **todas** as expressões sejam verdadeiras
- **OU**: basta que **uma** seja verdadeira
- **NÃO**: inverte o valor lógico da expressão

Operadores adicionais citados (sem aprofundamento): NOR, NAND, XOR.

### Expressões

- **Matemáticas**: combinam valores e operadores aritméticos; sintaxe deve ser obedecida
- **Relacionais/lógicas**: usadas geralmente em condições de estruturas de controle de fluxo (`SE ... ENTÃO`)

Exemplos:
```
SOMA <- 3 + 5
MEDIA <- (VALOR1 + VALOR2) / 2
RESULTADO <- 5 + (3 * 2 - (1 + 4))   // resultado = 6
SE (IDADE >= 18) ENTÃO
SE (VALOR > 0 E VALOR < 10) ENTÃO
```

### Precedência de Operadores

1. **Parênteses** (mais internos primeiro)
2. `*`, `/`, `%` (multiplicação, divisão, resto)
3. `+`, `-` (soma, subtração)
4. Operadores **relacionais** (todos com mesmo nível, executados após os aritméticos)
5. Operadores **lógicos**

---

## Conexões com o que já existe na wiki

- [Operadores e Expressões](../conceitos/operadores-e-expressoes.md) — conceito central desta aula
- [Pseudocódigo](../conceitos/pseudocodigo.md) — expressões fazem parte da sintaxe do pseudocódigo
- [Palavras Reservadas](../conceitos/palavras-reservadas.md) — `SE`, `ENTÃO` são palavras reservadas usadas com expressões relacionais/lógicas

---

## Perguntas abertas

- Como a precedência de operadores se relaciona com a implementação nos compiladores (análise sintática)?
