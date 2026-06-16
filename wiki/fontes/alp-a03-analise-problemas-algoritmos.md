---
titulo: "ALP A03 — Análise de Problemas e Elaboração de Soluções Computacionais usando Algoritmos"
tipo: fonte
tags: [algoritmo, software, hardware, compilacao, interpretacao, bytecode, historia]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-a03-analise-problemas-algoritmos]
criado: 2026-05-28
atualizado: 2026-05-28
---

# ALP A03 — Análise de Problemas e Elaboração de Soluções Computacionais usando Algoritmos

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Algoritmos e Lógica de Programação |
| Aula | 03 |
| Ingerida em | 2026-05-28 |

---

## Resumo

A aula contextualiza historicamente o desenvolvimento de software e algoritmos, desde os autômatos mecânicos e a teoria das linguagens formais (1950) até a popularização dos computadores pessoais e interfaces gráficas. Em seguida, detalha as três formas de execução de programas: interpretada, compilada e híbrida (bytecode).

---

## Pontos-chave

### Contexto histórico

- **Ada Lovelace** (1840s): tradutora e anotadora do artigo de Menabrea; suas anotações são consideradas o primeiro programa de computador da história
- **Teoria das linguagens formais** (década de 1950): base para análise léxica/sintática e desenvolvimento de linguagens artificiais precursoras das linguagens de programação
- **Computador pessoal** (1980s): IBM e Apple popularizaram hardware de bom desempenho, tamanho e preço acessíveis — explosão da indústria de software
- **GUI**: XEROX (1970s) → Apple Lisa/Macintosh (1980s) → MS-DOS/Windows 1.0 (1985) → Windows 3.0/3.11 (1990s); cada etapa abriu novos nichos de desenvolvimento de software
- Software passou de interação direta com hardware → interação com sistema operacional → aplicações de propósito geral

### Codificação e Execução de Programas

Existem três formas de se executar um programa:

| Tipo | Processo | Exemplos |
|------|----------|---------|
| **Interpretado** | Código-fonte → interpretador executa diretamente, sem conversão intermediária | JavaScript em navegadores, HTML |
| **Compilado** | Código-fonte → compilador → arquivo objeto → linkador → executável nativo independente | C, C++ |
| **Híbrido (bytecode)** | Código-fonte → compilador → arquivo intermediário → interpretador (máquina virtual) executa | Java (JVM) |

- Cada plataforma exige um compilador específico; sem compilador, o SO não consegue gerar executáveis para determinada linguagem
- No método híbrido são necessários dois softwares (compilador + interpretador), o que tende a aumentar o tempo de execução

---

## Conexões com o que já existe na wiki

- [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md) — conceito central desta aula; ALP A03 apresenta o mesmo conteúdo que LP A3, porém de ângulo introdutório (sem nomenclatura técnica de lexemas/tokens)
- [Linguagem C](../conceitos/linguagem-c.md) — exemplo de linguagem compilada
- [Linguagem Java](../conceitos/linguagem-java.md) — exemplo canônico do método híbrido (bytecode/JVM)
- [Paradigma Estruturado](../conceitos/paradigma-estruturado.md) — software que segue estruturação sequencial de instruções

---

## Perguntas abertas

- A aula cita Ada Lovelace como autora do primeiro programa de computador — vale criar página de autora?
- A teoria das linguagens formais (1950s) remete a Chomsky e Turing — criar página para esses autores?
