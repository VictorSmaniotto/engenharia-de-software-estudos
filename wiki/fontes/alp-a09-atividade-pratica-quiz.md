---
titulo: "ALP A9 — Atividade Prática: Quiz em Portugol"
tipo: fonte
tags: [algoritmo, pseudocódigo, portugol, visualg, estruturas-de-repeticao, estruturas-de-decisao, vetores]
disciplina: Algoritmos e Lógica de Programação
fontes: []
criado: 2026-06-02
atualizado: 2026-06-02
---

# ALP A9 — Atividade Prática: Quiz em Portugol

## Metadados

- **Disciplina:** Algoritmos e Lógica de Programação
- **Tipo:** Atividade prática avaliativa
- **Ferramenta:** VisuAlg (arquivo .txt em Portugol)
- **Data de ingestão:** 2026-06-02

## Resumo

Atividade de desenvolvimento de um algoritmo de quiz de perguntas e respostas com sistema de pontuação e avaliação de desempenho. O aluno deve escrever o algoritmo em pseudocódigo (Portugol), executável no VisuAlg.

## Regras do jogo (enunciado)

- 5 perguntas sobre Algoritmos e Lógica de Programação
- Cada pergunta permite até **2 tentativas**:
  - 1ª tentativa correta → **10 pontos**
  - 2ª tentativa correta → **5 pontos**
  - Erra as duas → **0 pontos**
- Pontuação máxima: 50 pontos
- Ao final, exibir mensagem conforme desempenho:
  - 50 pts → "EXCELENTE"
  - 37–49 pts → "ÓTIMO"
  - 25–36 pts → "BOM"
  - < 25 pts → "RUIM"

## Pontos-chave da solução

- **Vetor de opções válidas** `opcoes[1..4]` com valores "a", "b", "c", "d" — centraliza validação de entrada
- **Variável `tentativas`** como controlador da estrutura `REPITA/ATÉ`: sobe para 3 quando acerta (encerra o loop), independente da tentativa
- **`ENQUANTO questoes <= 5 FACA`** — laço externo que itera pelas 5 questões
- **`REPITA/ATÉ tentativas = 3`** — laço interno que controla as tentativas de cada questão
- **`Minusc(resposta)`** — normalização da entrada para evitar erros por maiúscula/minúscula
- **SE aninhados** — 5 blocos `SE questoes = N ENTAO` definem cada questão
- Validação de entrada inválida: se a resposta não estiver no vetor de opções, exibe "Resposta inválida!"

## Conceitos praticados

- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md): ENQUANTO e REPITA/ATÉ aninhados
- [Estruturas de Decisão](../conceitos/estruturas-de-decisao.md): SE simples e aninhado
- [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md): vetor de caracteres para opções válidas
- [Entrada e Saída de Dados](../conceitos/entrada-e-saida-de-dados.md): LEIA, ESCREVA, ESCREVAL
- [Palavras Reservadas](../conceitos/palavras-reservadas.md): sintaxe Portugol completa

## Conexões com a wiki

- Integra todos os conceitos de ALP vistos até a A8 em um único programa funcional
- Demonstra na prática a combinação de laços aninhados com controle de estado (variável `tentativas`)
