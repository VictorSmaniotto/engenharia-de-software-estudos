---
titulo: "Linguagens de Programação — Aula 2: Classificação de Paradigmas"
tipo: fonte
tags: [paradigmas, classificacao, criterios-de-linguagens, sebesta]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-07
atualizado: 2026-05-07
---

# LP — Aula 2: Classificação de Paradigmas

**Disciplina:** [Linguagens de Programação](../disciplinas/linguagens-de-programacao.md)
**Aula:** 2
**Arquivo original:** `raw/Classificação de  Paradigmas.md`
**Referência principal:** [Sebesta (2011)](../autores/sebesta.md)

---

## Resumo

A aula apresenta como as linguagens de programação são avaliadas segundo critérios de Sebesta (2011) e estabelece a classificação formal dos paradigmas em três categorias principais: **imperativo, funcional e lógico** — com OO como derivação do imperativo.

---

## Pontos-chave

### Critérios de avaliação de linguagens (Sebesta, 2011)

Três critérios principais, cada um composto por características:

| Critério | Características associadas |
|----------|---------------------------|
| **Legibilidade** | Simplicidade, ortogonalidade, tipos de dados, projeto da sintaxe |
| **Facilidade de escrita** | Simplicidade, ortogonalidade, abstração, expressividade |
| **Confiabilidade** | Verificação de tipos, tratamento de exceções, legibilidade, facilidade de escrita |

**Características relevantes:**
- **Simplicidade**: contribui para os três critérios; pouca variedade de estruturas básicas
- **Ortogonalidade**: menor número de combinações entre estruturas → menos ambiguidade e exceções. C tem baixa ortogonalidade por causa dos ponteiros.
- **Abstração**: capacidade de definir em processos e estruturas as características relevantes de um problema real
- **Expressividade**: simplificação de expressões e variedade de comandos (ex: múltiplos tipos de laço)
- **Verificação de tipos em compilação** é melhor que em tempo de execução (custo de processamento)

### Classificação dos paradigmas (Sebesta, 2011)

**Três categorias principais:**

1. **[Imperativo](../conceitos/paradigma-imperativo.md)** — execução ordenada de instruções; inclui o estruturado
   - Derivação: **[Orientação a Objetos](../conceitos/paradigma-oo.md)** (abstração de dados em classes)
   - Scripts (JavaScript, Ruby, Perl) são basicamente imperativos
   - Linguagens visuais (Visual Basic, Delphi) derivam de imperativos textuais

2. **[Funcional](../conceitos/paradigma-funcional.md)** — perspectiva matemática; imutabilidade; funções de comportamento fixo; facilita reutilização e escala

3. **[Lógico](../conceitos/paradigma-logico.md)** — programação baseada em regras sem ordem de execução definida; regras formam base de conhecimento que gera novas informações

**Outras variantes mencionadas:**
- Orientada a eventos, orientada a aspectos (derivadas de OO)
- Declarativa (HTML, SQL)
- Baseada em blocos (Scratch, Blocky)
- Programação dinâmica (quebra problemas em subproblemas; usa recursividade)

### Citação importante

> "O bom programador não é aquele que conhece várias linguagens, mas aquele que sabe pensar em bons algoritmos eficientes e conhece uma boa linguagem para aplicar a estes algoritmos."

---

## Conexões com a Wiki

- **Expande** [Paradigma Funcional](../conceitos/paradigma-funcional.md): acrescenta a distinção de imutabilidade vs. mutabilidade do imperativo
- **Expande** [Paradigma OO](../conceitos/paradigma-oo.md): OO agora classificado como derivação do imperativo
- **Cria** [Paradigma Imperativo](../conceitos/paradigma-imperativo.md): categoria que engloba estruturado + scripts + linguagens visuais
- **Cria** [Paradigma Lógico](../conceitos/paradigma-logico.md): Prolog, Lisp (em contexto lógico)
- **Cria** [Critérios de Avaliação de Linguagens](../conceitos/criterios-avaliacao-linguagens.md): framework Sebesta

## Perguntas Abertas

- Como a recursividade será aprofundada nas próximas aulas?
- O material de Sebesta diferencia "estruturado" de "imperativo" ou os trata como sinônimos?
- Qual a posição de linguagens multiparadigma (Python, Scala) nessa classificação?
