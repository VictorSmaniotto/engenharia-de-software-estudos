---
titulo: Aninhamento de Estruturas de Controle
tipo: conceito
tags: [aninhamento, encadeamento, decisao, repeticao, teste-de-mesa]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula09-aninhamento-estruturas]
criado: 2026-06-15
atualizado: 2026-06-15
---

# Aninhamento de Estruturas de Controle

## Definição

Aninhamento (ou encadeamento) é a inserção de uma estrutura de controle dentro de outra, de forma que a estrutura interna só seja avaliada/executada sob as condições impostas pela estrutura externa.

## Tipos de Aninhamento

### Decisão dentro de Decisão
Um `SE` colocado dentro de outro `SE`; a estrutura interna é alcançada apenas se a condição externa for `VERDADEIRO`.

```
SE (A >= B) ENTÃO
  SE (A >= C) ENTÃO
    ESCREVA ("A PODE SER O MAIOR VALOR");
  SENÃO
    ESCREVA ("C PODE SER O MAIOR VALOR");
  FIMSE;
FIMSE;
```

### Repetição dentro de Repetição
Dois ou mais laços aninhados; o laço interno completa um ciclo inteiro a cada iteração do externo. Exemplo: hodômetro de três dígitos (000–999) com três `PARA` aninhados.

### Repetição dentro de Decisão
Um laço de repetição só é executado se uma condição `SE` for satisfeita.

### Decisão dentro de Repetição
Uma estrutura `SE` é avaliada a cada iteração; pode ser usada para alterar variáveis de controle e forçar saída antecipada do laço.

## Teste de Mesa

Técnica apresentada por Manzano (1997) para validar algoritmos antes de executá-los: monta-se uma tabela com amostras de dados de entrada e registra-se o resultado esperado do algoritmo para cada amostra. Detecta erros lógicos sem necessidade de execução real.

| A | B | C | Resultado esperado |
|---|---|---|--------------------|
| 1 | 2 | 3 | C PODE SER O MAIOR |
| 3 | 2 | 1 | A PODE SER O MAIOR |

## Cuidados

- Cada nível de aninhamento adiciona complexidade lógica; um planejamento prévio do fluxo reduz erros.
- Estrutura interna depende da externa: o resultado da condição externa define se o bloco interno é ou não alcançado.

## Relações

- [Estruturas de Decisão](estruturas-de-decisao.md)
- [Estruturas de Repetição](estruturas-de-repeticao.md)
- [Vetores e Matrizes](vetores-e-matrizes.md) — manipulação de matrizes 2D exige laços aninhados obrigatoriamente
