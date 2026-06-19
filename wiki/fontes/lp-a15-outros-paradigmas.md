---
titulo: LP A15 — Outros Paradigmas e Formas de Programação
tipo: fonte
tags: [linguagens, eventos, aspectos, programacao-dinamica, grafos, arduino, aspectj, blocos]
disciplina: Linguagens de Programação
fontes: [lp-a15-outros-paradigmas]
criado: 2026-06-18
atualizado: 2026-06-18
---

# LP A15 — Outros Paradigmas e Formas de Programação

- **Disciplina:** Linguagens de Programação
- **Aula:** 15 — Outros Paradigmas e Formas de Programação
- **Fonte original:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-15.html
- **Ingerida em:** 2026-06-18

## Resumo

Encerra o módulo apresentando paradigmas e formas de programação que surgiram a partir dos quatro tradicionais ou para necessidades específicas: **orientado a eventos**, **orientado a aspectos** e **programação dinâmica**. Inclui ainda a **programação em blocos** (Scratch/Blockly) e noções de **teoria de grafos**.

## Pontos-chave

### Programação orientada a eventos
- Trata a interação do software com **eventos** via rotinas de tratamento de **gatilhos** (entradas, eventos de software ou do sistema operacional). Não é necessariamente extensão do OO, mas pode usar seus conceitos (ex.: C#).
- Usa *design patterns* (modelos de solução já testados, não código pronto). Típico de **interfaces gráficas**: cliques, teclas, toques, entradas automatizadas.
- Eventos esperados são tratados pelo software; inesperados, pelo sistema operacional. Quanto mais completo o tratamento, mais robusta a aplicação.
- Fluxo de execução diferente do imperativo/OO: não há fluxo contínuo determinado pelo processamento; o software reage a eventos que podem ocorrer de forma imprevisível — ou nunca ocorrer. Existe uma rotina principal que aguarda eventos e é interrompida para tratá-los.
- Exemplos: Visual Basic, Visual C, Delphi (desktop com GUI); C#, Java, JavaScript (eventos em formulários web). **Arduino** (versão própria de C) usa laço infinito `loop()` interrompido por eventos; `setup()` configura a placa.
- **Programação em blocos** (Scratch, Blockly): montagem gráfica por encaixe; extremamente didática para ensinar lógica (estruturas do paradigma imperativo); blocos podem ser traduzidos para outras linguagens.

### Programação orientada a aspectos
- Organiza o código segundo sua **relevância** nos requisitos, complementando o OO. Desenvolvida por **Gregor Kiczales** e equipe na **Xerox PARC**.
- **AspectJ**: linguagem que não cria aplicações completas, mas **complementos para Java** (analogia com PHP/JavaScript ligados a HTML/CSS). Permite encapsular código secundário/transversal em módulos (**aspectos**).
- **Aspect weaver**: ferramenta que age como compilador, unindo o código principal aos aspectos pelo processo de **weaving**, gerando o *bytecode* para a JVM.
- Mecanismos: `pointcut` (desvio com o `join point` que liga classe e aspecto), `call`, e `before` (executa conteúdo antes do método principal — comparado a um desvio incondicional, como o antigo GOTO). Útil para agrupar tratamento de erros e código transversal.

### Programação dinâmica
- Reduz problemas complexos a subproblemas de menor complexidade, otimizando o desenvolvimento. Trata partes fracionadas como completas, desde que integráveis na solução original.
- Apoia-se na **teoria de grafos** (rotas logísticas: vértices = pontos, arestas = caminhos, **pesos** = custos) — representável como diagrama, vetor ou matriz.
- Adequada a problemas que exigem **adaptação a eventos** e baixa previsibilidade: controle de estoque (e-commerce), rotas de GPS (recalculadas por acidentes, obras, erros do motorista). Trabalha com **estados** do processo.
- **Clojure** aceita programação dinâmica: mesmo sendo tipada, os tipos não são verificados na compilação; estruturas em listas podem ser manipuladas em tempo de execução.

## Conexões com a wiki

- Origina os conceitos [Programação Orientada a Eventos](../conceitos/programacao-orientada-a-eventos.md), [Programação Orientada a Aspectos](../conceitos/programacao-orientada-a-aspectos.md), [Programação Dinâmica](../conceitos/programacao-dinamica.md) e [Teoria de Grafos](../conceitos/teoria-de-grafos.md).
- Origina o autor [Gregor Kiczales](../autores/kiczales.md).
- Aspectos + bytecode/JVM conectam-se a [Linguagem Java](../conceitos/linguagem-java.md) e [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md).
- Clojure dinâmico complementa [Linguagem Clojure](../conceitos/linguagem-clojure.md).

## Perguntas abertas

- Programação dinâmica aqui aproxima-se de "otimização adaptativa" — como se relaciona com a técnica algorítmica clássica de mesmo nome (memoização)?
- Orientação a eventos é paradigma ou estilo arquitetural?
