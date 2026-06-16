---
titulo: "ALP A08 — Estruturas de Repetição"
tipo: fonte
tags: [estruturas-de-repeticao, enquanto, repita, para, laco, iteracao, contador]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a08-estruturas-de-repeticao]
criado: 2026-05-28
atualizado: 2026-05-28
---

# ALP A08 — Estruturas de Repetição

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Algoritmos e Lógica de Programação |
| Aula | 08 |
| Ingerida em | 2026-05-28 |

---

## Resumo

A aula apresenta as três estruturas de repetição do pseudocódigo: condicional com verificação no início (`ENQUANTO...FAÇA`), condicional com verificação no fim (`REPITA...ATÉ`) e contada (`PARA...DE...ATÉ...PASSO...FAÇA`). Discute o papel da variável de controle, o risco de laço infinito e as diferenças práticas entre as opções.

---

## Pontos-chave

### Por que usar estruturas de repetição?

- Elimina a necessidade de repetir código manualmente
- Permite que algoritmos realizem tarefas repetitivas com menos linhas
- Pode conter dentro do laço outras estruturas (`SE`, `ESCOLHA`, outros laços)
- Controle via **variável contadora** ou via mudança de estado de dados

---

### 1. Repetição Condicional — `ENQUANTO...FAÇA...FIMENQUANTO`

Condição verificada **antes** de cada iteração — pode **não executar nenhuma vez** se a condição já for falsa na entrada.

```
CONTADOR <- 1;
ENQUANTO (CONTADOR <= 100) FAÇA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
  CONTADOR <- CONTADOR + 1;
FIMENQUANTO;
```

- Importante: **inicializar** a variável de controle antes do laço
- Dentro do laço deve haver instrução que **modifique a condição**, senão → **laço infinito**

---

### 2. Repetição Condicional — `REPITA...ATÉ`

Condição verificada **após** cada iteração — executa **ao menos uma vez**.

```
CONTADOR <- 1;
REPITA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
  CONTADOR <- CONTADOR + 1;
ATÉ (CONTADOR > 100);
```

- A condição do `REPITA...ATÉ` é de **parada** (o laço para quando a condição é verdadeira)
- A condição do `ENQUANTO` é de **continuidade** (o laço continua enquanto verdadeira)
- Mesma lógica, lados opostos: `<= 100` no ENQUANTO ↔ `> 100` no REPITA

---

### 3. Repetição Contada — `PARA...DE...ATÉ...PASSO...FAÇA...FIMPARA`

Quantidade de iterações **predefinida** no próprio comando.

```
PARA CONTADOR DE 1 ATÉ 100 PASSO 1 FAÇA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
FIMPARA;
```

Parâmetros:
| Palavra-chave | Função |
|--------------|--------|
| `PARA` + variável | define a variável de controle |
| `DE` | valor inicial |
| `ATÉ` | valor final (condição de parada) |
| `PASSO` | incremento/decremento a cada iteração |
| `FAÇA` | inicia o bloco de instruções |
| `FIMPARA` | encerra a estrutura |

**Variante flexível** (controle externo ao comando `PARA`):

```
CONTADOR <- 1;
PARA CONTADOR ATÉ 100 FAÇA
  ESCREVA ("ITERAÇÃO ", CONTADOR);
  CONTADOR <- CONTADOR + 1;
FIMPARA;
```

---

### Comparativo

| Estrutura | Condição | Executa sem entrar? | Melhor uso |
|-----------|----------|---------------------|-----------|
| `ENQUANTO` | Início | Sim (pode não executar) | Quantidade desconhecida; condição prévia |
| `REPITA` | Final | Não (mínimo 1 vez) | Deve executar ao menos uma vez |
| `PARA` | Início (predefinida) | Sim (pode não executar) | Quantidade de iterações conhecida |

---

## Conexões com o que já existe na wiki

- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md) — conceito central desta aula
- [Estruturas de Decisão](../conceitos/estruturas-de-decisao.md) — podem ser aninhadas dentro de laços
- [Operadores e Expressões](../conceitos/operadores-e-expressoes.md) — condições dos laços usam operadores relacionais
- [Variáveis e Constantes](../conceitos/variaveis-e-constantes.md) — variável de controle/contador
- [Palavras Reservadas](../conceitos/palavras-reservadas.md) — ENQUANTO, FAÇA, FIMENQUANTO, REPITA, ATÉ, PARA, DE, PASSO, FIMPARA
