---
titulo: "LP A9 — POO: Outras Linguagens (Smalltalk e C++)"
tipo: fonte
tags: [poo, smalltalk, cpp, orientado-a-objetos, bytecode, multiparadigma]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-19
atualizado: 2026-05-19
---

# LP A9 — POO: Outras Linguagens (Smalltalk e C++)

## Metadados

- **Disciplina:** Linguagens de Programação
- **Aula:** 09
- **Data de ingestão:** 2026-05-19
- **URL:** https://ead.unimar.br/aulas/linguagens-de-programacao/aula-09.html

## Resumo

Apresenta duas linguagens que implementam o paradigma OO: Smalltalk (que nasceu junto com o paradigma) e C++ (que adicionou OO ao C estruturado, tornando-se multiparadigma). Menciona também diferenças nos modificadores de acesso da linguagem C#.

## Pontos-chave

### Smalltalk

- Linguagem que **nasceu junto com o paradigma OO** — referência histórica central
- Introduziu a interação com usuários via janelas (GUI) — Wangenheim (2002)
- **Tudo é objeto**: inclusive as classes, que são instâncias de *metaclasses* → não precisam ser instanciadas separadamente
- Compilação para **bytecode** interpretado por máquina virtual — conceito que influenciou diretamente o Java
- **Herança simples apenas** — tudo da superclasse é automaticamente herdado
- Polimorfismo: duas classes distintas podem ter o mesmo nome de método em superclasse e subclasse
- *Case sensitive* (como C e Java)
- Tipos numéricos são objetos: `10` → `Smallinteger`, `23.90` → float, `7/3` → `Fraction`
- Sintaxe própria: `timesRepeat`, `to:by:do:`, `whileTrue`, `whileFalse`
- Delimitadores: `""` para comentários, `''` para strings, `[]` para blocos, `|` para variáveis, `.` como terminador
- Boa **ortogonalidade** (baixa redundância)

### C++

- C com OO adicionado → **linguagem multiparadigma** (estruturado + OO)
- Mesmos modificadores de acesso de Java: `public`, `protected`, `private`
- Separação código/definição em dois arquivos: `.hpp` (cabeçalho — define classe) e `.cpp` (implementação)
- `#include "arquivo.hpp"` liga os arquivos em tempo de compilação
- **Construtores**: mesmo nome da classe, inicializa atributos; criados via `new`
- **Destrutores**: prefixo `~` antes do nome da classe; chamado ao fim da vida do objeto

### C# (menção)

- Modificadores além de public/protected/private: `internal`, `internal protected`, `protected private`
- Exemplo de variação possível no nível de encapsulamento entre linguagens OO

## Conexões com a Wiki

- [Paradigma OO](../conceitos/paradigma-oo.md)
- [Linguagem Java](../conceitos/linguagem-java.md) — bytecode/JVM tem origem em Smalltalk
- [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md) — bytecode
- [Encapsulamento](../conceitos/encapsulamento.md) — modificadores em C++ e C#
- [Herança](../conceitos/heranca.md) — herança simples em Smalltalk
- [Polimorfismo](../conceitos/polimorfismo.md)
- [Linguagem Smalltalk](../conceitos/linguagem-smalltalk.md)
- [Linguagem C++](../conceitos/linguagem-cpp.md)

## Perguntas Abertas

- Qual é a diferença prática entre metaclasse em Smalltalk e classe abstrata em Java?
- C++ moderno (C++11/17) expandiu o paradigma funcional — quais mecanismos?
