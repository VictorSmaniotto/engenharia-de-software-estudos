---
titulo: Sub-Rotinas (Procedimentos e Funções)
tipo: conceito
tags: [sub-rotina, procedimento, funcao, modularizacao, paradigma-estruturado, escopo, retorno]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula13-sub-rotinas, alp-aula14-parametros, alp-aula15-recursividade]
criado: 2026-06-15
atualizado: 2026-06-15
---

# Sub-Rotinas (Procedimentos e Funções)

## Definição

Uma **sub-rotina** é um bloco de instruções com nome próprio e certa independência funcional. Pode ser chamada a partir do algoritmo principal ou de outras sub-rotinas, evitando duplicação de código e permitindo reutilização.

A introdução de sub-rotinas corresponde ao uso do **paradigma estruturado** — em contraste com o paradigma imperativo puro, onde toda a lógica fica em um único bloco sequencial.

## Tipos

### Procedimento
Sub-rotina **sem retorno de valor**. Acessa variáveis globais diretamente; chamado simplesmente pelo nome.

```
PROCEDIMENTO CALCULA ()
  DECLARE INTEIRO: SOMA;
  SOMA <- V1 + V2 + V3;
  ESCREVA ("RESULTADO = ", SOMA);
FIM;
```

*V1, V2, V3 precisam ser globais ou passadas como parâmetros.*

### Função
Sub-rotina **com tipo de retorno**. Usa `RETORNE` para devolver um valor ao chamador; deve ser usada em atribuição, expressão ou `ESCREVA`.

```
FUNÇÃO CALCULA () DE INTEIRO
  DECLARE INTEIRO: SOMA;
  SOMA <- V1 + V2 + V3;
  RETORNE SOMA;
FIM;
```

## Escopo

| Declaração | Escopo | Duração |
|-----------|--------|---------|
| No algoritmo principal | Global — acessível em qualquer ponto | Toda a execução |
| Dentro de uma sub-rotina | Local — invisível externamente | Apenas durante a execução da sub-rotina |

Dados locais são **perdidos** ao sair da sub-rotina. Para preservá-los, usar [passagem por referência](passagem-de-parametros.md) ou retorno de função.

## Terminologia

- **Forbellone (2005):** usa "módulo" para toda sub-rotina.
- **Manzano (1997):** distingue procedimentos de funções — convenção adotada no material ALP.
- **Ascencio (2011):** sintaxe similar ao material; influência na padronização adotada.

## Recursividade

Uma sub-rotina pode chamar a si mesma — ver [Recursividade](recursividade.md).

## Relações

- [Passagem de Parâmetros](passagem-de-parametros.md)
- [Escopo](escopo.md)
- [Recursividade](recursividade.md)
- [Paradigma Estruturado](paradigma-estruturado.md)
- [Paradigma Funcional](paradigma-funcional.md) — funções são a unidade central do paradigma funcional
