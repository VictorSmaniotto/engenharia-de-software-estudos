---
titulo: Paradigma Funcional (Programação Funcional)
tipo: conceito
tags: [paradigma, funcional, lisp, haskell, clojure, funcoes-puras, imutabilidade]
disciplina: Linguagens de Programação
fontes: [lp-m2-a01-paradigmas-de-programacao, lp-a02-classificacao-de-paradigmas, lp-a10-programacao-funcional-conceitos, lp-a11-programacao-funcional-clojure, lp-a12-programacao-funcional-outras-linguagens]
criado: 2026-05-07
atualizado: 2026-06-18
---

# Paradigma Funcional

## Definição

Uma das três categorias principais de paradigmas segundo Sebesta (2011). Traz uma perspectiva **matemática** para a programação: toda a codificação se baseia no conceito de **função matemática** (relação entre domínio e imagem). Dados são constantes, funções têm comportamento fixo e **evita-se ao máximo mudança de estado** — ao contrário do [imperativo](paradigma-imperativo.md), onde estados mudam constantemente.

> "As linguagens funcionais trazem uma perspectiva mais matemática para a programação com dados constantes e funções de comportamento fixo que facilita a reutilização e ampliação de aplicações de forma escalar em função da não mutabilidade destas funções." (LP A2)

Tem raízes na linguagem **Lisp** (1950–60s), criada com foco em Inteligência Artificial (LP M2 A1).

## Conceitos centrais

### Funções puras e imutabilidade

Uma **função pura** recebe parâmetros e sempre retorna o mesmo resultado para a mesma entrada — sem depender de estado externo. Ver [Funções Puras e Imutabilidade](funcoes-puras.md).

### Lambda

**Alonzo Church** (1940s) definiu o termo **lambda** para funções não nomeadas. Adotado pelo paradigma e por linguagens multiparadigma modernas (ex.: Java 8+).

### Tipos de dados (Lisp)

Apenas dois tipos básicos: **átomos** (numéricos ou alfanuméricos) e **listas** (delimitadas por parênteses, podendo conter átomos ou outras listas).
- Ex.: `(1 2 3 (4 5) 6)` — 4 átomos + 1 sublista = 5 elementos

### Notação prefixa (polonesa)

Operador vem **antes** dos operandos: `(+ 3 4)` ao invés de `3 + 4`. Ver [Notação Prefixa](notacao-prefixa.md).

### Recursividade no funcional puro

Linguagens funcionais puras (Sebesta, 2011) **não usam variáveis nem atribuições** → sem laços de repetição → substituídos por **recursividade**. Compiladores modernos podem converter recursões em iterações para ganhar desempenho.

## Funcional puro vs. geral

| Tipo | Exemplos | Características |
|------|----------|----------------|
| **Puro** | [Haskell](linguagem-haskell.md), ML | Sem variáveis, sem atribuição, sem laços; recursividade obrigatória |
| **Geral** | Clojure, ML, [Scheme](linguagem-scheme.md) | Agrega variáveis e outros recursos; maior versatilidade |

> Nota (LP A12): ML aparece nos dois lados conforme o recorte — é funcional, com sintaxe próxima das demais linguagens, e serve de contraste a Haskell, cuja sintaxe lembra sistemas de equações matemáticas.

## Linguagens representativas

| Linguagem | Época | Nota |
|-----------|-------|------|
| [Lisp](linguagem-lisp.md) | 1950–60s | Pioneira; átomos e listas; base para IA |
| [Scheme](linguagem-scheme.md), ML | 1970s | Derivadas de Lisp; funções como valores/elementos de listas |
| [Haskell](linguagem-haskell.md) | 1980s | Funcional puro; sintaxe matemática |
| [Clojure](linguagem-clojure.md) | 2000s | JVM + concorrência; usado no Nubank |

## Multiparadigma: o funcional agregado ao OO

O funcional não vive só em linguagens dedicadas. Linguagens modernas o **agregam** ao orientado a objetos (LP A12):
- **[Kotlin](linguagem-kotlin.md)** (JetBrains): permite funções fora de classes → código puramente funcional.
- **Java (8+)**: incorpora lambda e recursos funcionais.
- **Python**: usa o multiparadigma OO + funcional de forma natural, com sintaxe limpa (`def par(x): return (x % 2) == 0`).

## Vantagens

- Menos linhas de código para o mesmo resultado
- Código mais fácil de testar, manter e evoluir
- Maior previsibilidade (funções puras)
- Suporte natural a concorrência e paralelismo (sem estado compartilhado mutável)

## Nota histórica

Lisp foi "base para estudos iniciais da chamada inteligência artificial" — conexão relevante com o ressurgimento do funcional em contextos de IA/ML modernos.

## Relações

- [Paradigma Estruturado](paradigma-estruturado.md)
- [Paradigma OO](paradigma-oo.md)
- [Funções Puras e Imutabilidade](funcoes-puras.md)
- [Notação Prefixa](notacao-prefixa.md)
- [Recursividade](recursividade.md)
- [Linguagem Lisp](linguagem-lisp.md), [Scheme](linguagem-scheme.md), [Haskell](linguagem-haskell.md), [Clojure](linguagem-clojure.md), [Kotlin](linguagem-kotlin.md)

## Fontes

- [LP M2 A1 — Paradigmas de Programação](../fontes/lp-m2-a01-paradigmas-de-programacao.md)
- [LP A2 — Classificação de Paradigmas](../fontes/lp-a02-classificacao-de-paradigmas.md)
- [LP A10 — Programação Funcional: Conceitos](../fontes/lp-a10-programacao-funcional-conceitos.md)
- [LP A11 — Programação Funcional: Linguagem Clojure](../fontes/lp-a11-programacao-funcional-clojure.md)
- [LP A12 — Programação Funcional: Outras Linguagens](../fontes/lp-a12-programacao-funcional-outras-linguagens.md)
