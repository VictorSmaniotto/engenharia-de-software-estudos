---
titulo: Linguagem Smalltalk
tipo: conceito
tags: [smalltalk, poo, bytecode, metaclasse, heranca-simples]
disciplina: Linguagens de Programação
fontes: [lp-a09-poo-outras-linguagens]
criado: 2026-05-19
atualizado: 2026-05-19
---

# Linguagem Smalltalk

## Definição

Linguagem que **nasceu junto com o paradigma orientado a objetos**, sendo referência histórica central do OO. Também introduziu a interação com usuários por janelas (GUI). Wangenheim (2002) é a referência principal.

## Características principais

- **Tudo é objeto** — inclusive as classes, que são instâncias de *metaclasses*; as classes não precisam ser instanciadas para criar objetos
- Objetos e instâncias são criados via envio de mensagem `new` (como em Java)
- **Herança simples** apenas: tudo da superclasse é automaticamente herdado pelas subclasses
- **Polimorfismo**: superclasse e subclasse podem ter métodos de mesmo nome
- **Compilação para bytecode** interpretado por máquina virtual — conceito que influenciou diretamente o Java
- *Case sensitive* (como C e Java): convenção — atributos/métodos iniciam em minúsculas, classes em maiúsculas
- Boa **ortogonalidade** (baixa redundância de código)

## Tipos de dados

Tipos numéricos são objetos (instâncias de classes numéricas):
- `10` → `Smallinteger`
- `23.90` → float
- `7/3` → `Fraction`

## Sintaxe característica

| Elemento | Símbolo/Palavra |
|----------|----------------|
| Comentário | `"texto"` (aspas duplas) |
| String | `'texto'` (aspas simples) |
| Bloco de comandos | `[ ... ]` |
| Delimitador de variáveis | `| var |` |
| Terminador de comando | `.` (ponto final) |
| Parâmetros | `:` (dois pontos) |

Estruturas de repetição:
- `timesRepeat`: número fixo de iterações
- `to:by:do:`: laço contado com início, fim e passo
- `whileTrue` / `whileFalse`: laços condicionais

## Contexto histórico

Foi uma das linguagens mais antigas que serviram de base para outras. Sua influência sobre Java é direta: bytecode, JVM e o uso de `new` para instanciar objetos.

## Relações

- [Paradigma OO](paradigma-oo.md) — linguagem fundadora do paradigma
- [Linguagem Java](linguagem-java.md) — herdou bytecode/JVM e `new` de Smalltalk
- [Herança](heranca.md) — apenas herança simples em Smalltalk
- [Polimorfismo](polimorfismo.md)
- [Compilação e Interpretação](compilacao-e-interpretacao.md) — bytecode

## Fontes

- [LP A9 — POO: Outras Linguagens](../fontes/lp-a09-poo-outras-linguagens.md)
