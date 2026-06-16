---
titulo: "LP A8 — POO: Linguagem Java"
tipo: fonte
tags: [java, poo, heranca, polimorfismo, encapsulamento, interfaces, classes-abstratas, package]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-11
atualizado: 2026-05-11
---

# LP A8 — POO: Linguagem Java

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Linguagens de Programação |
| Aula | 8 |
| Fonte original | https://ead.unimar.br/aulas/linguagens-de-programacao/aula-08.html |
| Data de ingestão | 2026-05-11 |

---

## Resumo

Apresenta Java como linguagem OO de referência. Detalha estrutura básica de código, tipos de dados, instanciação de objetos, e os três pilares do OO em Java (`extends`, `private`/`public`/`protected`, `@Override`). Avança para classes abstratas (`abstract`), interfaces (`interface`/`implements`) e herança múltipla via interfaces (Java 8+).

---

## Pontos-chave

### Estrutura Básica
- Organização em **pacotes** (`package`): agrupa classes de uma mesma aplicação em um mesmo escopos
- Importação de classes externas: `import java.util.Scanner`
- Ponto de entrada: método `main(String[] args)` — único método que não precisa de objeto instanciado
- Todo código dentro de classes; programação puramente estruturada não é possível
- Linguagem compilada para **bytecode** (.class) interpretado pela JVM (ver [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md))

### Tipos de Dados
- Primitivos: `int`, `float`, `char`, `boolean` — mesmos do C
- Estruturas complexas simplificadas: `ArrayList` para listas de objetos (não aceita primitivos diretamente)
- Tipos evoluíram ao longo das versões para simplificar manipulação de dados

### Instanciação de Objetos
- Declaração: `NomeDaClasse nomeObjeto;`
- Instanciação: `nomeObjeto = new NomeDaClasse();` — chama o construtor
- Acesso a métodos: `nomeObjeto.nomeMetodo()` — sempre prefixado pelo objeto ao qual se refere
- Variáveis dentro de métodos ≠ atributos de classe: atributos são declarados fora dos métodos

### Encapsulamento em Java
- `private`: atributo/método acessível apenas dentro da própria classe
- `public`: visível por qualquer classe do pacote
- `protected`: visível por subclasses; recomendado para manter encapsulamento com herança

### Herança em Java
- Palavra reservada `extends`: `class Subclasse extends Superclasse`
- Subclasse acessa atributos e métodos `protected` da superclasse
- Uma classe pode ser `public` (dominante) + outra `default` ou `private` no mesmo arquivo (com restrições)

### Polimorfismo em Java
- Método de mesmo nome redefinido na subclasse com `@Override`
- `@Override`: informa ao compilador que o método sobrescreve um da superclasse; gera erro se o nome não existir na superclasse (auxilia manutenção de código)

### Classes Abstratas
- `abstract class`: serve apenas como modelo para subclasses; **não pode ser instanciada**
- Métodos `abstract`: declarados sem implementação na superclasse; obrigatoriamente implementados nas subclasses
- Uso: quando a superclasse define estrutura mas não tem implementação própria útil

### Interfaces
- `interface`: tipo especial de classe abstrata — apenas declarações de métodos (sem implementação)
- Implementada por classes via `implements`: `class Agricultor implements Profissao`
- `@Override` também usado com interfaces
- Atributos de interface: implicitamente `static` e `final`
- Uso: permite **herança múltipla** — uma classe pode implementar várias interfaces
- A partir de Java 8: métodos `default` em interfaces permitem implementação padrão

### Diferença: Classe Abstrata vs Interface

| | Classe Abstrata | Interface |
|--|----------------|-----------|
| Instanciável? | Não | Não |
| Pode ter implementação? | Sim (métodos concretos) | Só com `default` (Java 8+) |
| Herança múltipla? | Não | Sim (`implements A, B`) |
| Palavra-chave | `extends` | `implements` |

---

## Conexões com o que já existe na wiki

- [Linguagem Java](../conceitos/linguagem-java.md): esta aula é a principal fonte desta página
- [Compilação e Interpretação](../conceitos/compilacao-e-interpretacao.md): bytecode/JVM mencionado em LP A3
- [Encapsulamento](../conceitos/encapsulamento.md), [Herança](../conceitos/heranca.md), [Polimorfismo](../conceitos/polimorfismo.md)
- [Classes Abstratas e Interfaces](../conceitos/classes-abstratas-interfaces.md)
- [Sebesta (2011)](../autores/sebesta.md): encapsulamento de nomeação via `package` citado

---

## Perguntas abertas

- Quando escolher classe abstrata vs interface para modelar hierarquia de classes?
- Como `ArrayList` e generics (`<T>`) se relacionam com o sistema de tipos do Java?
