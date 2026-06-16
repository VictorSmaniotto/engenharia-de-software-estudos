---
titulo: "ALP A06 — Entrada e Saída de Dados"
tipo: fonte
tags: [entrada-de-dados, saida-de-dados, leia, escreva, algoritmo, interatividade]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a06-entrada-e-saida-de-dados]
criado: 2026-05-28
atualizado: 2026-05-28
---

# ALP A06 — Entrada e Saída de Dados

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Algoritmos e Lógica de Programação |
| Aula | 06 |
| Ingerida em | 2026-05-28 |

---

## Resumo

A aula apresenta os mecanismos de interação entre usuário e algoritmo: entrada de dados via teclado (`LEIA`) e saída de dados em tela (`ESCREVA`). Apresenta boas práticas de nomenclatura de variáveis e validação de entrada. Encerra com um algoritmo completo que calcula a média entre três valores.

---

## Pontos-chave

### Entrada de Dados — `LEIA`

- Sintaxe: `LEIA (VARIAVEL);` — aguarda digitação do usuário (via teclado)
- Permite múltiplas variáveis em uma instrução: `LEIA (PESO, ALTURA);`
- Cada dado inserido deve ser confirmado com ENTER

```
LEIA (X);
LEIA (IDADE);
LEIA (PESO, ALTURA);
```

**Boas práticas:**
- Usar **nomes intuitivos** para variáveis (ex: `PESO_MAXIMO`, `PESOMAXIMO` em vez de `X`)
- Espaços não são permitidos em identificadores — use `_` para separar palavras compostas
- **Validar entradas**: ex., impedir divisor zero verificando o valor recebido antes de usar

### Saída de Dados — `ESCREVA`

- Sintaxe: `ESCREVA (parâmetros);` — exibe dados em tela
- Aceita: **mensagens de texto** (entre aspas) e **variáveis** (pelo nome), misturados
- Múltiplos parâmetros separados por `,` são **concatenados** na exibição

```
ESCREVA ("Texto Exemplo");
ESCREVA (IDADE);
ESCREVA (PESO, " – ", ALTURA);
ESCREVA ("Nome: ", NOME);
ESCREVA ("O valor da média entre ", VALOR1, " e ", VALOR2, " é: ", MEDIA);
```

- Textos entre aspas podem conter qualquer caractere (maiúsculas, minúsculas, símbolos, números)
- Variáveis exibem o valor armazenado (sem aspas)
- Cuidado com espaçamento nos textos ao redor de variáveis para evitar concatenação sem separação visual

### Algoritmo Completo — Cálculo de Média

```
INÍCIO
DECLARE
  REAL VALOR1, VALOR2, VALOR3, MEDIA;
  ESCREVA ("DIGITE UM PRIMEIRO VALOR: ");
  LEIA (VALOR1);
  ESCREVA ("DIGITE UM SEGUNDO VALOR: ");
  LEIA (VALOR2);
  ESCREVA ("DIGITE UM TERCEIRO VALOR: ");
  LEIA (VALOR3);
  MEDIA <- (VALOR1 + VALOR2 + VALOR3) / 3;
  ESCREVA ("A MÉDIA ENTRE OS TRÊS VALORES É ", MEDIA);
FIM.
```

Padrão de interação típico: alternância de `ESCREVA` (instrução ao usuário) + `LEIA` (coleta do dado).

---

## Conexões com o que já existe na wiki

- [Entrada e Saída de Dados](../conceitos/entrada-e-saida-de-dados.md) — conceito central desta aula
- [Variáveis e Constantes](../conceitos/variaveis-e-constantes.md) — variáveis são o destino dos dados lidos
- [Operadores e Expressões](../conceitos/operadores-e-expressoes.md) — expressão `(V1+V2+V3)/3` exemplifica o uso
- [Palavras Reservadas](../conceitos/palavras-reservadas.md) — `LEIA` e `ESCREVA` são palavras reservadas

---

## Perguntas abertas

- Como se implementa validação de entrada em pseudocódigo? (uso de estruturas de decisão — ver A07)
