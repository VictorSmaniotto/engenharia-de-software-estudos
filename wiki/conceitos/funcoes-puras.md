---
titulo: Funções Puras e Imutabilidade
tipo: conceito
tags: [funcional, funcoes-puras, imutabilidade, efeitos-colaterais, lambda]
disciplina: Linguagens de Programação
fontes: [lp-a10-programacao-funcional-conceitos]
criado: 2026-05-19
atualizado: 2026-05-19
---

# Funções Puras e Imutabilidade

## Definição

Uma **função pura** é aquela que, dados os mesmos parâmetros de entrada, **sempre retorna o mesmo resultado** — independentemente do estado externo. É o princípio central do paradigma funcional e deriva da noção matemática de função (domínio → imagem).

## Imutabilidade

A **imutabilidade** é a propriedade da função pura: seu comportamento é fixo para uma dada entrada. Não há variação de resultado causada por estado externo.

> "Uma função que recebe um valor multiplica esse valor por ele mesmo e retorna este resultado é imutável, pois sempre que um valor for passado como parâmetro, o mesmo resultado do valor ao quadrado será retornado." (LP A10)

## O que torna uma função impura?

| Causa de impureza | Exemplo |
|-------------------|---------|
| Variável global usada internamente | Cotação de moeda lida de variável externa |
| Arquivo como parâmetro | Conteúdo pode mudar entre execuções |
| Número aleatório interno | Resultado varia a cada chamada |
| Atribuição a estrutura de dados externa | Efeito colateral no estado global |

## Efeitos colaterais

São ações que uma função realiza além de retornar um valor — principalmente **alterar estruturas de dados fora de si mesma** sem passar pelo retorno. O funcional puro elimina efeitos colaterais ao máximo.

## Benefícios das funções puras

- Mais previsíveis e confiáveis
- Mais fáceis de **testar** (resultado conhecido para cada entrada)
- Mais fáceis de **reutilizar** e integrar
- Facilitam leitura e compreensão do código

## Lambda (funções não nomeadas)

**Alonzo Church** (década de 1940) definiu o termo **lambda** para funções sem nome — conceito adotado pelo paradigma funcional e por linguagens multiparadigma como **Java 8+**.

## Linguagem funcional pura vs. geral

| Tipo | Características |
|------|----------------|
| **Pura** (ex.: Haskell) | Sem variáveis, sem atribuição, sem laços → usa recursividade |
| **Geral** (ex.: Clojure) | Agrega variáveis e outros recursos → maior versatilidade, menor desempenho puro |

Compiladores modernos podem converter recursões em estruturas iterativas (*tail-call optimization*) para compensar a diferença de desempenho.

## Relações

- [Paradigma Funcional](paradigma-funcional.md) — contexto maior
- [Notação Prefixa](notacao-prefixa.md) — sintaxe de chamada de funções no funcional
- [Recursividade](recursividade.md) — substitui laços de repetição no funcional puro
- [Linguagem Clojure](linguagem-clojure.md) — implementação concreta com dados imutáveis
- [Escopo](escopo.md) — variáveis globais vs. locais; causa de impureza

## Fontes

- [LP A10 — Programação Funcional: Conceitos](../fontes/lp-a10-programacao-funcional-conceitos.md)
