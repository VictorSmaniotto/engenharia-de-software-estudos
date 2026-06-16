---
titulo: "Cartão de Estudos 01 — ALP e LP"
tipo: sintese
tags: [revisao, algoritmos, paradigmas, linguagens, criterios-de-avaliacao]
fontes: [alp-a01-conceitos-gerais-de-programacao, alp-a02-classificacao-de-algoritmos, lp-m2-a01-paradigmas-de-programacao, lp-a02-classificacao-de-paradigmas]
criado: 2026-05-07
atualizado: 2026-05-07
---

# Cartão de Estudos 01 — ALP e LP

Cobre as 4 aulas ingeridas até 2026-05-07: ALP A1, ALP A2, LP M2 A1 e LP A2.

---

## Algoritmo e Lógica de Programação

**#1 — O que é um algoritmo e qual a diferença entre ele e um programa?**

Um algoritmo é uma representação em idioma local de uma possível solução computacional — visa a compreensão lógica, não a execução direta. Precisa ser convertido em uma linguagem de programação para se tornar software executável.

---

**#2 — Quais são as três formas de representar soluções computacionais? Qual tem maior proximidade com código?**

Descrição narrativa (frases curtas, baixo detalhe), fluxograma (diagrama com formas padronizadas, mais intuitivo) e pseudocódigo/Portugol (maior detalhamento, mais próximo de linguagens de programação). O pseudocódigo tem maior proximidade com código.

---

**#3 — Quais são as duas seções básicas de um algoritmo em pseudocódigo?**

Seção de declaração (`DECLARE` — estruturas de dados e tipos) e seção principal (instruções de entrada, processamento e saída).

---

**#4 — O que é uma palavra reservada? Por que ela existe tanto em pseudocódigo quanto em linguagens de programação?**

Palavra com significado fixo que não pode ser usada para outro fim. Em linguagens reais, é necessária para que compiladores e interpretadores consigam processar as instruções.

---

**#5 — Quais são os quatro tipos de algoritmos segundo a classificação por paradigma? Qual é o mais indicado para iniciantes?**

Sequencial/imperativo, estruturado, orientado a objetos e lógico/funcional. O sequencial é o mais indicado para iniciantes por ter lógica mais simples e maior quantidade de material de pesquisa disponível.

---

**#6 — O que é recursividade e qual é o elemento obrigatório para que funcione corretamente?**

Técnica em que uma sub-rotina chama a si mesma repetidamente com novos dados. O elemento obrigatório é a **condição de parada** — sem ela, a recursão é infinita.

---

**#7 — Cite dois algoritmos clássicos de ordenação e qual deles usa recursividade.**

Bubble sort e merge sort. O merge sort usa recursividade (dividir para conquistar).

---

## Linguagens de Programação

**#8 — Segundo Sebesta (2011), quais são as três categorias principais de paradigmas de programação?**

Imperativo, funcional e lógico. A orientação a objetos é uma **derivação** do imperativo, não uma categoria principal.

---

**#9 — Qual a diferença fundamental entre o paradigma imperativo e o funcional no tratamento de estado?**

No imperativo, os estados mudam constantemente durante a execução. No funcional, adota-se **imutabilidade** — dados são constantes e funções têm comportamento fixo.

---

**#10 — O que caracteriza o paradigma lógico e como ele difere do imperativo?**

No lógico, o programa é definido como um conjunto de regras **sem ordem de execução predefinida** — o sistema infere resultados a partir da base de regras. No imperativo, o programador define passo a passo *como* chegar ao resultado.

---

**#11 — Quais são os três critérios de avaliação de linguagens de programação de Sebesta?**

Legibilidade (facilidade de compreender o código), facilidade de escrita (facilidade de desenvolver soluções) e confiabilidade (capacidade de o software se comportar corretamente).

---

**#12 — O que é ortogonalidade em uma linguagem de programação? Cite um exemplo de linguagem com baixa ortogonalidade.**

Ortogonalidade é o grau de regularidade das combinações entre estruturas — alta ortogonalidade significa poucas exceções e comportamentos inesperados. **C** tem baixa ortogonalidade por causa dos ponteiros, que geram um grande número de combinações possíveis.

---

**#13 — Por que a verificação de tipos em tempo de compilação é preferível à verificação em tempo de execução?**

Porque tem menor custo de processamento — erros de tipo são detectados antes da execução, sem consumir recursos do programa em funcionamento.

---

**#14 — Qual linguagem dos anos 1950–60 serviu de base para os estudos iniciais de Inteligência Artificial? Qual paradigma ela representa?**

**Lisp** (LISt Processor). Representa o paradigma funcional — e é também a raiz de linguagens como Scheme, ML e Clojure.

---

**#15 — Conexão transversal: paradigma estruturado e paradigma imperativo — qual a relação entre eles segundo as duas disciplinas?**

O imperativo é a **categoria principal** (Sebesta, LP A2); o estruturado é um **subtipo** do imperativo que adiciona a subdivisão em sub-rotinas (PROCEDIMENTO/FUNÇÃO) que se comunicam por troca de dados. Em ALP, o algoritmo estruturado é apresentado como evolução do sequencial puro.

---

## Páginas relacionadas

- [Pseudocódigo](../conceitos/pseudocodigo.md)
- [Fluxograma](../conceitos/fluxograma.md)
- [Palavras Reservadas](../conceitos/palavras-reservadas.md)
- [Recursividade](../conceitos/recursividade.md)
- [Algoritmos de Ordenação](../conceitos/algoritmos-de-ordenacao.md)
- [Paradigma Imperativo](../conceitos/paradigma-imperativo.md)
- [Paradigma Estruturado](../conceitos/paradigma-estruturado.md)
- [Paradigma Funcional](../conceitos/paradigma-funcional.md)
- [Paradigma Lógico](../conceitos/paradigma-logico.md)
- [Paradigma OO](../conceitos/paradigma-oo.md)
- [Critérios de Avaliação de Linguagens](../conceitos/criterios-avaliacao-linguagens.md)
