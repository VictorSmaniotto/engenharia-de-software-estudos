---
titulo: "LP A10 — Programação Funcional: Conceitos"
tipo: fonte
tags: [funcional, funcoes-puras, imutabilidade, lambda, lisp, notacao-prefixa]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-19
atualizado: 2026-05-19
---

# LP A10 — Programação Funcional: Conceitos

## Metadados

- **Disciplina:** Linguagens de Programação
- **Aula:** 10
- **Data de ingestão:** 2026-05-19
- **URL:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-10.html

## Resumo

Apresenta os fundamentos matemáticos do paradigma funcional: conceito de função (domínio → imagem), funções puras, imutabilidade, efeitos colaterais, lambda (Alonzo Church, 1940s), tipos de dados em Lisp (átomos e listas) e notação prefixa/polonesa. Discute vantagens em testabilidade, reuso e manutenção.

## Pontos-chave

- **Base matemática**: função = relação entre elementos de um conjunto domínio e um conjunto imagem
- **Paradigma não imperativo**: execução não é sequencial como no imperativo; ordem definida pelas operações
- Linguagens representativas: Lisp, ML, Scheme, Haskell — base do paradigma; podem agregar outros paradigmas
- **Funções puras (imutáveis)**: dado o mesmo parâmetro, sempre retornam o mesmo resultado → previsíveis e sem efeitos colaterais
  - Função impura: usa variável externa além dos parâmetros → resultado pode variar
  - Causas de impureza: variáveis globais, arquivos como parâmetros, números aleatórios
- **Efeitos colaterais**: alterações em estruturas de dados fora da função → problema central do funcional
- **Lambda**: termo definido por **Alonzo Church (1940s)** para funções não nomeadas → adotado pelo paradigma e por linguagens multiparadigma (ex.: Java 8+)
- **Linguagem funcional pura** (Sebesta, 2011): não usa variáveis nem instruções de atribuição → sem laços de repetição → substituídos por **recursividade**
  - Recursão é mais lenta que iteração, mas compiladores modernos convertem recursões em estruturas iterativas
- **Tipos em Lisp**: apenas dois — átomos (numéricos ou alfanuméricos) e listas (entre parênteses, contendo átomos ou outras listas)
  - Ex.: `(1 2 3 (4 5) 6)` — 4 átomos + 1 sublista = 5 elementos
- **Notação prefixa (polonesa)**: operador antes dos operandos — ex.: `(+ 3 4)` ao invés de `3 + 4`
- Funções primitivas: base para construção de funções complexas
- Vantagens do funcional: menos linhas de código, mais fácil de manter/testar/evoluir, maior previsibilidade

## Conexões com a Wiki

- [Paradigma Funcional](../conceitos/paradigma-funcional.md)
- [Funções Puras e Imutabilidade](../conceitos/funcoes-puras.md)
- [Notação Prefixa](../conceitos/notacao-prefixa.md)
- [Recursividade](../conceitos/recursividade.md) — substitui laços de repetição no funcional puro
- [Sebesta (2011)](../autores/sebesta.md)

## Perguntas Abertas

- Como o Java 8 implementou lambdas — quais limitações em relação a linguagens funcionais puras?
- Quais compiladores realmente convertem recursões em iterações (tail-call optimization)?
