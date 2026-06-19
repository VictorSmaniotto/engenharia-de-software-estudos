---
titulo: LP A14 — Programação Lógica: Linguagem Prolog
tipo: fonte
tags: [linguagens, logico, prolog, fatos, regras, instancias, comutatividade, recursividade]
disciplina: Linguagens de Programação
fontes: [lp-a14-programacao-logica-prolog]
criado: 2026-06-18
atualizado: 2026-06-18
---

# LP A14 — Programação Lógica: Linguagem Prolog

- **Disciplina:** Linguagens de Programação
- **Aula:** 14 — Programação Lógica: Linguagem Prolog
- **Fonte original:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-14.html
- **Ingerida em:** 2026-06-18

## Resumo

A aula apresenta a **linguagem Prolog**, representante do [paradigma lógico](../conceitos/paradigma-logico.md). O foco é construir bases de **fatos** e **regras** sobre objetos por meio de **relações** (proposições atômicas), testá-las com consultas, e entender o problema da **comutatividade** das relações. Mostra também variáveis, recursividade implícita na busca e cálculos em tempo de execução.

## Pontos-chave

- No paradigma lógico pensa-se em **o que serve de base** para o processamento, não em **como** os dados são processados (contraste com imperativo/estruturado).
- **Proposições atômicas**: relações que incidem sobre **termos** (equivalentes aos átomos de Lisp), em listas entre parênteses separadas por vírgulas. Cada linha é uma **instância**; o conjunto de instâncias define a relação.
- **Comutatividade**: `amigo(ana, marcos)` ≡ `amigo(marcos, ana)` porque a relação amizade é comutativa. Já `chefe(ana, marcos)` ≠ `chefe(marcos, ana)`, pois chefia não é comutativa. O interpretador **não entende o sentido do nome** da relação — só importam as instâncias definidas.
- **Consultas**: `? amigo(X, Y).` lista todas as instâncias (variáveis em aberto). Se `marcos` aparece só como segundo termo, `? amigo(marcos, Y).` retorna `false` — para corrigir, é preciso **adicionar as instâncias com termos invertidos**, "ensinando" a comutatividade ao interpretador.
- **Sintaxe de termos**: **constantes** iniciam com letra **minúscula**; **variáveis** iniciam com letra **maiúscula**.
- Plataforma de teste citada: SWISH (https://swish.swi-prolog.org/).
- Exemplo de **árvore genealógica** mescla relações comutativas (`irmãos`) e não-comutativas (`pai`, `mae`). Irmãos aparecem duas vezes nas consultas por causa da comutatividade.
- **Cálculo em tempo de execução**: base `pessoa(Nome, Horas, Salário)`; consulta `? pessoa(X,Y,Z), Media is Z/Y.` calcula a média salarial por hora, armazenando o resultado na variável `Media`.
- **Aplicações** de Prolog: computação simbólica (prova automática de teoremas), bancos de dados relacionais, linguagem natural, solucionadores de jogos e **sistemas especialistas**.

## Conexões com a wiki

- Origina o conceito [Linguagem Prolog](../conceitos/linguagem-prolog.md).
- Aplica concretamente os fundamentos de [Lógica Formal](../conceitos/logica-formal.md) e [Paradigma Lógico](../conceitos/paradigma-logico.md) (LP A13).
- Termos × átomos: ponte explícita com [Linguagem Lisp](../conceitos/linguagem-lisp.md).
- Sistemas especialistas e IA conectam-se à nota histórica de Lisp/IA no [Paradigma Funcional](../conceitos/paradigma-funcional.md).

## Perguntas abertas

- Como Prolog implementa recursividade explícita em regras (não apenas a busca interna)?
- Qual o papel do backtracking na geração de múltiplas soluções?
