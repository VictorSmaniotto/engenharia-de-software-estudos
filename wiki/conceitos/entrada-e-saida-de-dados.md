---
titulo: Entrada e Saída de Dados
tipo: conceito
tags: [entrada-de-dados, saida-de-dados, leia, escreva, interatividade, algoritmo]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a06-entrada-e-saida-de-dados]
criado: 2026-05-28
atualizado: 2026-05-28
---

# Entrada e Saída de Dados

## Definição

Entrada e saída de dados são os mecanismos que permitem a **interação entre usuário e algoritmo**. A entrada traz dados externos para dentro do algoritmo; a saída envia resultados e mensagens ao usuário.

---

## Entrada de Dados — `LEIA`

Coleta dados digitados pelo usuário (via teclado) e os armazena em variáveis.

```
LEIA (VARIAVEL);
LEIA (PESO, ALTURA);    ← múltiplas variáveis separadas por vírgula
```

- Cada dado inserido é confirmado com ENTER
- Outros meios de entrada (não tratados na disciplina): arquivos em disco, redes, Internet

---

## Saída de Dados — `ESCREVA`

Exibe informações em tela — mensagens fixas e/ou valores de variáveis.

```
ESCREVA ("Mensagem fixa");
ESCREVA (VARIAVEL);
ESCREVA ("Rótulo: ", VARIAVEL);
ESCREVA ("Entre ", V1, " e ", V2, " a média é: ", MEDIA);
```

- Textos entre aspas: qualquer caractere; não são palavras reservadas nem identificadores
- Parâmetros separados por `,` são **concatenados** na exibição
- Incluir espaços nos textos ao redor de variáveis para melhor legibilidade da saída
- Outros meios de saída: arquivo em disco, redes, web

---

## Boas Práticas

- **Nomear variáveis com clareza**: `PESO_MAXIMO` em vez de `X`
- Espaços são proibidos em identificadores; use `_` para palavras compostas
- **Validar entradas**: verificar o dado recebido antes de usá-lo (ex.: impedir divisor zero)
- Alternar `ESCREVA` (instrução) + `LEIA` (coleta) para orientar o usuário

---

## Algoritmo Padrão

```
ESCREVA ("INFORME O VALOR: ");
LEIA (VALOR);
```

Esse par é o padrão de interação mais comum em algoritmos com entrada de dados.

---

## Relações

- [Variáveis e Constantes](variaveis-e-constantes.md) — variáveis recebem os dados lidos por `LEIA`
- [Tipos de Dados](tipos-de-dados.md) — o tipo da variável define que dados são aceitos
- [Operadores e Expressões](operadores-e-expressoes.md) — expressões calculadas antes da saída com `ESCREVA`
- [Estruturas de Decisão](estruturas-de-decisao.md) — validação de entradas usa condicionais
- [Palavras Reservadas](palavras-reservadas.md) — `LEIA` e `ESCREVA` são palavras reservadas

## Fontes

- [ALP A06 — Entrada e Saída de Dados](../fontes/alp-a06-entrada-e-saida-de-dados.md)
