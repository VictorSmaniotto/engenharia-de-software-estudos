---
titulo: Critérios de Avaliação de Linguagens de Programação
tipo: conceito
tags: [linguagens, avaliacao, legibilidade, confiabilidade, sebesta]
disciplina: Linguagens de Programação
fontes: [lp-a02-classificacao-de-paradigmas]
criado: 2026-05-07
atualizado: 2026-05-07
---

# Critérios de Avaliação de Linguagens de Programação

## Definição

Framework de Sebesta (2011) para comparar e avaliar linguagens de programação segundo três critérios principais e suas características.

## Os Três Critérios

### 1. Legibilidade
Facilidade de compreender um código escrito na linguagem.

Características associadas: simplicidade, ortogonalidade, tipos de dados e estruturas, projeto da sintaxe.

### 2. Facilidade de Escrita
Facilidade de usar a linguagem para desenvolver soluções.

Características associadas: simplicidade, ortogonalidade, abstração, expressividade.

### 3. Confiabilidade
Capacidade de o software produzido se comportar corretamente.

Características associadas: verificação de tipos, tratamento de exceções, legibilidade, facilidade de escrita.

> Legibilidade e facilidade de escrita influenciam diretamente a confiabilidade.

## Características-chave

**Simplicidade** — contribui para os três critérios; pouca variedade de estruturas básicas reduz ambiguidade.

**Ortogonalidade** — menor número de combinações possíveis entre estruturas → menos exceções e comportamentos inesperados. Exemplo negativo: os ponteiros de C reduzem a ortogonalidade pela quantidade de combinações que permitem.

**Abstração** — capacidade de modelar características relevantes de um problema real em processos e estruturas de dados.

**Expressividade** — variedade de comandos que simplificam a codificação (ex: múltiplos tipos de laço de repetição).

**Verificação de tipos em compilação** — preferível à verificação em tempo de execução pelo menor custo de processamento.

**Tratamento de exceções** — melhora a garantia de funcionamento do software.

## Autor

[Sebesta (2011)](../autores/sebesta.md)

## Fontes

- [LP A2 — Classificação de Paradigmas](../fontes/lp-a02-classificacao-de-paradigmas.md)
