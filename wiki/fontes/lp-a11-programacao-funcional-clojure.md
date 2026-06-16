---
titulo: "LP A11 — Programação Funcional: Linguagem Clojure"
tipo: fonte
tags: [funcional, clojure, jvm, lisp, notacao-prefixa, concorrencia]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-19
atualizado: 2026-05-19
---

# LP A11 — Programação Funcional: Linguagem Clojure

## Metadados

- **Disciplina:** Linguagens de Programação
- **Aula:** 11
- **Data de ingestão:** 2026-05-19
- **URL:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-11.html

## Resumo

Apresenta Clojure como linguagem funcional moderna baseada em Lisp e na JVM. Cobre suas características principais: dados imutáveis, funções primitivas, notação prefixa, integração com Java, suporte a concorrência/paralelismo e carregamento de código em tempo de execução.

## Pontos-chave

- **Clojure**: linguagem funcional baseada em Lisp, roda na JVM; inspirada em Ruby, Python, Java e Haskell
- **Interpretada** — rodando na JVM tem acesso a todas as bibliotecas Java
- Aplicações Clojure e Java podem ser empacotadas juntas
- **Dados imutáveis (átomos)** e funções primárias — controle forte de mudanças de estado
- Suporte nativo a **concorrência e paralelismo** (múltiplas CPUs, múltiplos núcleos, computação distribuída) — Emerick (2012)
- **Carregamento de código em tempo de execução** → permite atualizações de missão crítica sem interrupção do serviço
- **Funções primitivas** principais:
  - `defn` — define uma função nomeada
  - `def` — define uma estrutura de dados (como um mapa/registro)
  - `apply` — aplica uma função a uma coleção
  - `count` — conta elementos de uma coleção
  - `let` — declara variáveis locais temporárias dentro de uma função
  - `cond` — estrutura condicional (equivale a switch/case)
- **Notação prefixa**: `(+ 3 4)` ao invés de `3 + 4`; operador sempre vem primeiro
- Operadores diferentes: `not` (≠ `!`), `inc` (≠ `++`)
- Estruturas de dados: listas com `[]` para parâmetros, `{}` para mapas rotulados (chave `:nome`)
- **Código menor**: mesmo resultado com menos linhas que estruturado ou OO equivalente
- **Caso de uso real**: ~90% dos microsserviços da Nubank são escritos em Clojure
- Variantes: `ClojureCLR` (.NET), `ClojureScript` (compila para JavaScript)
- Alternativa de entrada no funcional: JavaScript (multiparadigma, mercado amplo)

### Exemplo: função média
```clojure
(defn media [numeros]
  (/ (apply + numeros) (count numeros)))
```

### Exemplo: mapa rotulado
```clojure
(def agenda {:nome "Fulano de Tal" :fone "3322-5566"})
(:nome agenda)  ; => "Fulano de Tal"
```

### Exemplo: hipotenusa (Sebesta, 2011)
```clojure
(defn hypot [x y]
  (let [x2 (* x x)
        y2 (* y y)]
    (Math/sqrt (+ x2 y2))))
```

## Conexões com a Wiki

- [Paradigma Funcional](../conceitos/paradigma-funcional.md)
- [Linguagem Clojure](../conceitos/linguagem-clojure.md)
- [Notação Prefixa](../conceitos/notacao-prefixa.md)
- [Funções Puras e Imutabilidade](../conceitos/funcoes-puras.md)
- [Linguagem Java](../conceitos/linguagem-java.md) — JVM compartilhada
- [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md) — JVM
- [Emerick (2012)](../autores/emerick.md)
- [Sebesta (2011)](../autores/sebesta.md)

## Perguntas Abertas

- Como Clojure implementa STM (Software Transactional Memory) para controle de estado concorrente?
- ClojureScript vs JavaScript funcional (Ramda, fp-ts) — qual é mais adotado?
