---
titulo: Recursividade
tipo: conceito
tags: [algoritmo, recursividade, sub-rotinas, iteracao]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-a02-classificacao-de-algoritmos, lp-a02-classificacao-de-paradigmas, lp-a12-programacao-funcional-outras-linguagens]
criado: 2026-05-07
atualizado: 2026-06-18
---

# Recursividade

## Definição

Técnica em que uma sub-rotina chama a si mesma repetidamente, com novos dados a cada chamada, até que uma **condição de parada** seja atingida e as chamadas encerrem.

> "Algoritmos que tratam de uma lógica mais complexa e evoluída do uso de sub-rotinas capazes de chamar a si mesmas de forma iterativa ou repetitiva [...] existe um controle da quantidade de iterações baseado em uma condição que muitas vezes envolve valores numéricos que ao serem atingidos, encerram as sucessivas chamadas." (ALP A2)

## Paradigmas que suportam recursividade

- [Estruturado](paradigma-estruturado.md) — via PROCEDIMENTO ou FUNÇÃO
- [Funcional](paradigma-funcional.md) — é central neste paradigma; substitui laços de repetição
- [Orientado a Objetos](paradigma-oo.md) — via métodos

## Aplicações típicas

- Algoritmos de divisão em subproblemas (dividir para conquistar)
- Percurso em estruturas de dados como árvores e grafos
- Cálculo de fatorial, sequência de Fibonacci

## Relações

- [Algoritmos de Ordenação](algoritmos-de-ordenacao.md) — merge sort usa recursividade
- [Paradigma Funcional](paradigma-funcional.md) — recursão substitui mutabilidade de estado

## Exemplos em Algoritmo (ALP Aula 15)

### Potência recursiva
```
FUNÇÃO POTENCIA (INTEIRO BASE, INTEIRO EXPOENTE) DE INTEIRO
  SE (EXPOENTE = 0) ENTÃO
    RETORNE 1;
  SENÃO
    RETORNE (BASE * POTENCIA(BASE, EXPOENTE-1));
  FIMSE;
FIM;
```
`POTENCIA(5, 3)` → 5 * (5 * (5 * 1)) = 125. Condição de parada: expoente = 0 retorna 1.

### Tabuada recursiva
Dois parâmetros: `VALOR1` (decrementado a cada chamada) e `VALOR2` (fixo). O `ESCREVA` ocorre na *volta* das chamadas, exibindo a tabuada em ordem crescente apesar do decremento.

## Exemplos em linguagens funcionais (LP A12)

A recursão no funcional segue a mesma premissa (decisão + condição de parada), apenas com sintaxe própria:

```scheme
; Scheme — fatorial
(define (fat n) (if (= n 0) 1 (* n (fat (- n 1)))))
```

```haskell
-- Haskell — fatorial em duas equações
fact 0 = 1
fact n = n * fact (n - 1)
```

Em [linguagens funcionais puras](paradigma-funcional.md) (sem variáveis nem laços), a recursividade é **obrigatória**. Compiladores modernos podem converter recursões em iterações para ganhar desempenho. Ver [Linguagem Scheme](linguagem-scheme.md) e [Linguagem Haskell](linguagem-haskell.md).

## Recursão vs. Iteração

A mesma potência pode ser implementada iterativamente com `PARA I DE 1 ATÉ EXPOENTE`. A versão iterativa é mais simples de raciocinar; a recursiva é mais elegante para problemas definidos naturalmente de forma recursiva. Ver [Sub-Rotinas](sub-rotinas.md).

## Fontes

- [ALP A2 — Classificação de Algoritmos](../fontes/alp-a02-classificacao-de-algoritmos.md)
- [LP A2 — Classificação de Paradigmas](../fontes/lp-a02-classificacao-de-paradigmas.md)
- [ALP Aula 15 — Recursividade](../fontes/alp-aula15-recursividade.md)
- [LP A12 — Programação Funcional: Outras Linguagens](../fontes/lp-a12-programacao-funcional-outras-linguagens.md)
