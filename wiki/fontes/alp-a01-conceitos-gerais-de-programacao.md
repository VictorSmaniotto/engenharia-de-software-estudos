---
titulo: "Algoritmos e Lógica de Programação — Aula 1: Conceitos Gerais de Programação"
tipo: fonte
tags: [algoritmo, pseudocodigo, fluxograma, palavras-reservadas, logica-de-programacao]
disciplina: Algoritmos e Lógica de Programação
fontes: []
criado: 2026-05-07
atualizado: 2026-05-07
---

# ALP — Aula 1: Conceitos Gerais de Programação

**Disciplina:** [Algoritmos e Lógica de Programação](../disciplinas/algoritmos-e-logica-de-programacao.md)
**Aula:** 1
**Arquivo original:** `raw/ingeridos/Conceitos Gerais de Programação.md`
**Autores de referência:** [Forbellone](../autores/forbellone.md), [Manzano](../autores/manzano.md)

---

## Resumo

Introdução ao conceito de algoritmo como etapa intermediária entre a modelagem de um problema e o código em linguagem de programação. Apresenta as três formas de representação de soluções computacionais, a estrutura básica de um algoritmo e um conjunto de palavras reservadas usado ao longo da disciplina.

---

## Pontos-chave

### O que é um algoritmo

Representação em idioma local de uma possível solução computacional — visa a **compreensão lógica** da solução, não a execução direta. Precisa ser convertido em linguagem de programação para se tornar software executável.

> "O mais importante nesta etapa do aprendizado [...] é a lógica utilizada para solucionar problemas e compreender a estrutura de um código." (ALP A1)

### Formas de representação de soluções

| Forma | Características |
|-------|----------------|
| **Descrição narrativa** | Frases curtas em idioma natural; fácil compreensão, baixo detalhamento |
| **[Fluxograma](../conceitos/fluxograma.md)** | Diagrama com formas padronizadas (retângulo=ação, losango=decisão); mais intuitivo |
| **[Pseudocódigo](../conceitos/pseudocodigo.md) (Algoritmo)** | Portugol; maior proximidade com linguagens de programação; usa palavras reservadas |

As três formas podem variar de acordo com a fonte — a padronização do material segue **Forbellone**.

### Estrutura básica de um algoritmo

```
INÍCIO
  DECLARE
    <estruturas de dados>
  <instruções>
FIM.
```

- Seção de declaração: tipos de dados e variáveis
- Seção principal: entradas, processamento, saídas e estruturas de controle

### Palavras reservadas

Conjunto definido para a disciplina (base: Manzano + Forbellone). Exemplos categorizados:

| Categoria | Palavras |
|-----------|----------|
| Estrutura | INÍCIO, FIM, DECLARE |
| Entrada/Saída | LEIA, ESCREVA |
| Condicional | SE, ENTÃO, SENÃO, FIMSE, CASO, FIMCASO |
| Repetição | ENQUANTO, PARA, REPITA, FAÇA, ATÉ, PASSO |
| Sub-rotinas | PROCEDIMENTO, FUNÇÃO |
| OO | CLASSE, ATRIBUTO, MÉTODO |
| Tipos de dados | INTEIRO, REAL, CARACTERE, CONJUNTO |

---

## Conexões com a Wiki

- Paradigmas mencionados (estruturado, OO) conectam com [LP — conceitos de paradigmas](../conceitos/paradigma-estruturado.md)
- Pseudocódigo e fluxograma são ferramentas transversais a todo o curso

## Perguntas Abertas

- Quais estruturas de controle (condicionais, laços) serão detalhadas nas próximas aulas?
- O material usa Portugol padrão ou uma variante própria?
