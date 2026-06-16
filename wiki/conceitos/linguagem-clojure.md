---
titulo: Linguagem Clojure
tipo: conceito
tags: [clojure, funcional, jvm, lisp, concorrencia, imutabilidade]
disciplina: Linguagens de Programação
fontes: [lp-a11-programacao-funcional-clojure]
criado: 2026-05-19
atualizado: 2026-05-19
---

# Linguagem Clojure

## Definição

Clojure é uma linguagem funcional moderna baseada em **Lisp**, que roda na **JVM (Java Virtual Machine)**. Foi criada combinando aspectos de Ruby, Python, Java e Haskell para resolver problemas práticos enfrentados por desenvolvedores dessas linguagens. Referência: Emerick (2012).

## Características principais

- **Interpretada** — roda na JVM; acesso a todas as bibliotecas Java
- Aplicações Clojure e Java podem ser **empacotadas juntas**
- **Dados imutáveis (átomos)** + funções primárias → controle forte de mudanças de estado
- Suporte nativo a **concorrência e paralelismo** (múltiplas CPUs, múltiplos núcleos, computação distribuída)
- **Carregamento de código em tempo de execução** → atualizações em sistemas de missão crítica sem interrupção
- Desempenho comparável ou superior a Java e Python para certos workloads (origem em Lisp)
- **Notação prefixa** (polonesa): `(+ 3 4)` ao invés de `3 + 4`

## Funções primitivas principais

| Função | Uso |
|--------|-----|
| `defn` | Define uma função nomeada |
| `def` | Define uma estrutura de dados (mapa, valor) |
| `apply` | Aplica uma função a uma coleção de argumentos |
| `count` | Conta os elementos de uma coleção |
| `let` | Declara variáveis locais temporárias dentro de uma função |
| `cond` | Estrutura condicional (equivalente a switch/case) |

## Estruturas de dados

```clojure
; lista/vetor — parâmetros de funções
[numeros]

; mapa rotulado — chaves com ":"
{:nome "Fulano" :fone "3322-5566"}

; acessar campo do mapa
(:nome agenda)  ; => "Fulano"
```

## Operadores diferentes do C

| C / Java | Clojure |
|----------|---------|
| `!` (negação) | `not` |
| `++` (incremento) | `inc` |

## Exemplos de código

**Média aritmética:**
```clojure
(defn media [numeros]
  (/ (apply + numeros) (count numeros)))
```

**Hipotenusa (Sebesta, 2011):**
```clojure
(defn hypot [x y]
  (let [x2 (* x x)
        y2 (* y y)]
    (Math/sqrt (+ x2 y2))))
```

**Calculadora com `cond`:**
```clojure
(defn calc [a b c]
  (cond
    (= b +) (soma a c)
    (= b -) (sub a c)
    (= b *) (mult a c)
    (= b /) (div a c)))
```

## Caso de uso real

~90% dos microsserviços da **Nubank** são escritos em Clojure — caso famoso de adoção em produção de larga escala.

## Variantes

- `ClojureCLR` — compila para plataformas .NET
- `ClojureScript` — compila para JavaScript

## Relações

- [Paradigma Funcional](paradigma-funcional.md) — paradigma base
- [Funções Puras e Imutabilidade](funcoes-puras.md) — fundamento da linguagem
- [Notação Prefixa](notacao-prefixa.md) — sintaxe central
- [Linguagem Java](linguagem-java.md) — JVM compartilhada; bibliotecas interoperáveis
- [Compilação e Interpretação](compilacao-e-interpretacao.md) — interpretada via JVM
- [Emerick (2012)](../autores/emerick.md)
- [Sebesta (2011)](../autores/sebesta.md)

## Fontes

- [LP A11 — Programação Funcional: Linguagem Clojure](../fontes/lp-a11-programacao-funcional-clojure.md)
