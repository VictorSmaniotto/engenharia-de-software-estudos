---
titulo: "LP A3 — Programação Estruturada: Conceitos"
tipo: fonte
tags: [programacao-estruturada, imperativo, sintaxe, semantica, compilacao, interpretacao]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-11
atualizado: 2026-05-11
---

# LP A3 — Programação Estruturada: Conceitos

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Linguagens de Programação |
| Aula | 3 |
| Título original | Aula 3 - Programação Estruturada - Conceitos |
| Data de ingestão | 2026-05-11 |

---

## Resumo

A aula traça a evolução do paradigma imperativo até o estruturado, explica os conceitos fundamentais de sintaxe e semântica, e detalha os processos de compilação e interpretação (incluindo a variante bytecode). Apresenta os componentes básicos de um código estruturado: sub-rotinas, variáveis, matrizes e bibliotecas.

---

## Pontos-chave

### Programação Imperativa
- Baseada na Máquina de Turing: entrada → processamento → saída; estado muda por comandos
- Linguagens históricas: Algol, Fortran, COBOL, depois C, Basic, Pascal
- Código como bloco único; desvios de fluxo via **GOTO** (referência a marcadores numéricos ou textuais)
- BASIC original: apenas 15 tipos de comandos, sintaxe simples, popularizou-se rapidamente

### Programação Estruturada
- Agrega os conceitos do imperativo e acrescenta **sub-rotinas**, estruturas de decisão e repetição
- Surgiu na década de 1950; presente até hoje na maioria das linguagens
- Linguagens estruturadas de referência: PHP, Perl, Go (Google); Pascal, C, BASIC
- Permite absorver outros paradigmas (OO) sem abandonar a base estruturada

### Conceitos Essenciais

**Sintaxe**
- Forma correta de construção de cada instrução (palavras reservadas + parâmetros obrigatórios/opcionais)
- Base necessária para compiladores e interpretadores processarem código

**Semântica**
- Avalia a **estrutura do código** como um todo: correta colocação das instruções dentro da lógica da linguagem
- Complementa a sintaxe: sintaxe verifica se a instrução está bem formada; semântica verifica se está no lugar certo

**Compilação** (conforme Sebesta, 2011)
1. **Análise léxica**: reúne caracteres em lexemas (palavras reservadas, identificadores, valores numéricos)
2. **Análise sintática**: usa unidades léxicas para gerar árvores léxicas; verifica construção dos comandos
3. **Análise semântica**: avalia a estrutura completa do código
4. **Geração do arquivo objeto**: elimina comentários, prepara estrutura para linkagem
5. **Linkador**: agrega bibliotecas externas ao objeto, gerando o executável final

**Interpretação**
- Código fonte analisado e executado diretamente (sem gerar executável independente)
- Variante 1: erros ignoráveis são descartados em tempo de execução (navegadores web)
- Variante 2: análise prévia completa antes da execução; pode gerar arquivos temporários intermediários

**Bytecode (compilação parcial)**
- Código fonte → arquivo **bytecode** (objeto portável)
- Bytecode é interpretado por uma **máquina virtual** (ex.: JVM na linguagem Java)
- Alta portabilidade: mesmo bytecode roda em qualquer plataforma com interpretador compatível
- Contraste com compilação clássica: executáveis nativos não são portáveis entre plataformas

### Componentes de um Código Estruturado

- **Blocos de comandos**: instruções com desvios condicionais e laços de repetição
- **Variáveis**: unidades simples de armazenamento
- **Matrizes**: estruturas de dados mais complexas
- **Sub-rotinas**: permitem reúso de código e independência entre partes
- **Bibliotecas**: arquivos com código pré-desenvolvido e testado (ex.: entrada/saída)

---

## Conexões com o que já existe na wiki

- Expande [Paradigma Imperativo](../conceitos/paradigma-imperativo.md) com detalhe sobre GOTO e Alan Turing
- Expande [Paradigma Estruturado](../conceitos/paradigma-estruturado.md) com definição mais rica
- Cria base para [Sintaxe e Semântica](../conceitos/sintaxe-e-semantica.md)
- Cria base para [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md)
- Sebesta (2011) citado diretamente na descrição do analisador sintático

---

## Perguntas abertas

- Qual é exatamente a diferença entre análise sintática e semântica em casos práticos?
- Como a variante bytecode da Java se posiciona frente aos critérios de avaliação de Sebesta (portabilidade)?
