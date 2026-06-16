---
titulo: "Algoritmo e Lógica de Programação — Aula 2: Classificação de Algoritmos"
tipo: fonte
tags: [algoritmo, classificacao, recursividade, ordenacao, paradigmas]
disciplina: Algoritmo e Lógica de Programação
fontes: []
criado: 2026-05-07
atualizado: 2026-05-07
---

# ALP — Aula 2: Classificação de Algoritmos

**Disciplina:** [Algoritmo e Lógica de Programação](../disciplinas/algoritmo-e-logica-de-programacao.md)
**Aula:** 2
**Arquivo original:** `raw/ingeridos/Classificação de Algoritmos.md`

---

## Resumo

Classificação dos algoritmos segundo os paradigmas de programação (sequencial/imperativo, estruturado, OO, lógico/funcional) com exemplos de pseudocódigo para cada um. Apresenta também técnicas de elaboração de algoritmos: divisão em subproblemas, reuso, algoritmos clássicos (ordenação, grafos) e heurística.

---

## Pontos-chave

### Classificação por paradigma

| Paradigma | Característica no algoritmo | Exemplo de pseudocódigo |
|-----------|----------------------------|------------------------|
| **[Imperativo/Sequencial](../conceitos/paradigma-imperativo.md)** | Instruções executadas da primeira à última, em ordem | `INÍCIO ... INSTRUÇÃO; ... FIM.` |
| **[Estruturado](../conceitos/paradigma-estruturado.md)** | Subdivide em sub-rotinas (PROCEDIMENTO/FUNÇÃO) que se comunicam | `PROCEDIMENTO TESTE() ... INÍCIO ... TESTE(); ... FIM.` |
| **[Orientado a Objetos](../conceitos/paradigma-oo.md)** | Abstração em CLASSES com ATRIBUTOS e MÉTODOS | `CLASSE EXEMPLO ... ATRIBUTO DADO; ... MÉTODO PROCESSA();` |
| **Lógico/Funcional** | Baseado em regras da lógica matemática; dados imutáveis | — (não exemplificado em pseudocódigo nesta aula) |

**Nota sobre estruturado vs. imperativo:** o material trata o imperativo sequencial como a forma mais básica e o estruturado como uma evolução — alinhado com a classificação de Sebesta (LP A2), onde estruturado é subtipo do imperativo.

### [Recursividade](../conceitos/recursividade.md)

Sub-rotinas que chamam a si mesmas iterativamente, controladas por uma condição de parada. Suportada nos paradigmas estruturado, funcional e OO.

### Técnicas de elaboração de algoritmos

- **Divisão em subproblemas** — fracionar o problema até que cada parte seja simples o suficiente; integrar depois
- **Reuso** — algoritmos podem ser usados dentro de outros algoritmos
- **Algoritmos clássicos:**
  - Ordenação: [bubble sort, merge sort](../conceitos/algoritmos-de-ordenacao.md)
  - Estruturas de grafos — aplicáveis a problemas reais de rotas e conexões
- **Heurística** — soluções cognitivas (não puramente racionais) que processam escolhas mais rapidamente, ignorando detalhes não essenciais

---

## Conexões com a Wiki

- Conecta diretamente com os conceitos de paradigmas de LP: [imperativo](../conceitos/paradigma-imperativo.md), [estruturado](../conceitos/paradigma-estruturado.md), [OO](../conceitos/paradigma-oo.md), [funcional](../conceitos/paradigma-funcional.md)
- [Recursividade](../conceitos/recursividade.md) foi mencionada em LP A2 (Sebesta) — esta aula dá o primeiro exemplo concreto
- Algoritmos de grafos e heurística apontam para tópicos de análise de algoritmos a serem explorados

## Perguntas Abertas

- Bubble sort e merge sort serão implementados em pseudocódigo nas próximas aulas?
- A disciplina cobrirá análise de complexidade (Big O)?
