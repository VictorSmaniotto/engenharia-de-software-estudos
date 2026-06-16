---
titulo: Estruturas de Repetição
tipo: conceito
tags: [estruturas-de-repeticao, enquanto, repita, para, laco, iteracao, contador, loop]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a08-estruturas-de-repeticao]
criado: 2026-05-28
atualizado: 2026-05-28
---

# Estruturas de Repetição

## Definição

Estruturas de repetição (laços/loops) permitem que um bloco de instruções seja executado **repetidas vezes** de forma controlada. Eliminam a necessidade de repetir código manualmente e são fundamentais para processamento automatizado e iterativo.

---

## Tipos

### 1. `ENQUANTO...FAÇA...FIMENQUANTO` — condicional, verificação no início

Condição avaliada **antes** de cada iteração → pode **não executar** se já for falsa na entrada.

```
CONTADOR <- 1;
ENQUANTO (CONTADOR <= 100) FAÇA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
  CONTADOR <- CONTADOR + 1;
FIMENQUANTO;
```

- Condição de **continuidade**: laço roda enquanto for verdadeira
- Exige inicialização da variável de controle **antes** do laço
- Dentro do laço deve haver instrução que altere a condição → evitar **laço infinito**

---

### 2. `REPITA...ATÉ` — condicional, verificação no final

Condição avaliada **após** cada iteração → executa **ao menos uma vez**.

```
CONTADOR <- 1;
REPITA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
  CONTADOR <- CONTADOR + 1;
ATÉ (CONTADOR > 100);
```

- Condição de **parada**: laço para quando a condição se torna verdadeira (lógica invertida em relação ao `ENQUANTO`)

---

### 3. `PARA...DE...ATÉ...PASSO...FAÇA...FIMPARA` — contada

Quantidade de iterações **predefinida** no próprio comando.

```
PARA CONTADOR DE 1 ATÉ 100 PASSO 1 FAÇA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
FIMPARA;
```

| Elemento | Função |
|----------|--------|
| `DE` valor | Valor inicial da variável de controle |
| `ATÉ` valor | Valor final (condição de parada) |
| `PASSO` valor | Incremento/decremento por iteração |

Variante com controle externo (omite `DE` e `PASSO`):

```
CONTADOR <- 1;
PARA CONTADOR ATÉ 100 FAÇA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
  CONTADOR <- CONTADOR + 1;
FIMPARA;
```

---

## Comparativo

| Estrutura | Posição da condição | Mínimo de execuções | Melhor uso |
|-----------|---------------------|---------------------|-----------|
| `ENQUANTO` | Início | 0 | Quantidade desconhecida; validação prévia necessária |
| `REPITA` | Final | 1 | Ao menos uma iteração garantida |
| `PARA` | Início (predefinida) | 0 | Quantidade de iterações conhecida de antemão |

---

## Cuidados

- **Laço infinito**: ocorre quando a condição de parada nunca é atingida — a variável de controle deve ser modificada dentro do laço
- **Inicialização**: sempre inicializar a variável de controle para evitar valores residuais em memória
- Laços podem conter `SE`, `ESCOLHA` e outros laços internos (aninhamento)

---

## Relações

- [Estruturas de Decisão](estruturas-de-decisao.md) — podem ser usadas dentro de laços
- [Operadores e Expressões](operadores-e-expressoes.md) — condições dos laços usam operadores relacionais
- [Variáveis e Constantes](variaveis-e-constantes.md) — variável de controle/contador
- [Palavras Reservadas](palavras-reservadas.md) — ENQUANTO, FAÇA, FIMENQUANTO, REPITA, ATÉ, PARA, DE, PASSO, FIMPARA

## Fontes

- [ALP A08 — Estruturas de Repetição](../fontes/alp-a08-estruturas-de-repeticao.md)
