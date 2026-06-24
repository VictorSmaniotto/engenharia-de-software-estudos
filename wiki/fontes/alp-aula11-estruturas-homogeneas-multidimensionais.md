---
titulo: "ALP Aula 11 — Estruturas Homogêneas Multidimensionais (Matrizes)"
tipo: fonte
tags: [matriz, multidimensional, estrutura-homogenea, tabuleiro, imagem]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-aula11-estruturas-homogeneas-multidimensionais]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 11 — Estruturas Homogêneas Multidimensionais (Matrizes)

**Disciplina:** Algoritmos e Lógica de Programação  
**Módulo/Aula:** Aula 11  
**Data de ingestão:** 2026-06-15

---

## Resumo

Amplia o conceito de vetor para **duas ou mais dimensões** (matrizes). Apresenta aplicações práticas (imagens, jogos de tabuleiro) e um algoritmo completo para o jogo da velha implementado no VisualG.

---

## Pontos-chave

- **Matriz como imagem:** tela 1024×768 pode ser representada como matriz de pixels, onde cada célula contém um valor de cor.
- **Jogos de tabuleiro:** xadrez, damas, jogo da velha — a posição de peças é naturalmente representada por linha×coluna em uma matriz.
- **Declaração (sintaxe Forbellone):**
  ```
  TIPO TABULEIRO = MATRIZ [1..8][1..8] DE CARACTERES;
  TIPO CUBOMAGICO = MATRIZ [1..3][1..3][1..3] DE INTEIRO;
  ```
  Cada par de colchetes `[1..N]` representa uma dimensão adicional.
- **Índices (linha, coluna):** acesso por `MATRIZ[I,J]` — dois índices para 2D. O VisualG usa vírgula; o padrão do material usa colchetes separados.
- **Aninhamento obrigatório:** percorrer matriz 2D exige dois `PARA` aninhados (externo = linhas, interno = colunas).
- **Exemplo — Jogo da Velha:** algoritmo completo com 3×3 de caracteres, variáveis de jogador e rodadas, inicialização com espaços, verificação de todas as combinações vencedoras para "X" e "O".
- **Ferramenta VisualG 3.0:** permite execução de algoritmos em português; desenvolvida por Antonio Carlos Nicolodi.

---

## Conceitos relacionados

- [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md)
- [Aninhamento de Estruturas](../conceitos/aninhamento-de-estruturas.md)
- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md)

---

## Perguntas abertas

- Como representar matrizes esparsas (maioria de células com valor padrão) de forma eficiente?
- Em linguagens modernas, qual é o equivalente do `TIPO MATRIZ = MATRIZ[...]` do Portugol?
