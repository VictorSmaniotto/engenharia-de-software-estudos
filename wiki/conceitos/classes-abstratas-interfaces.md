---
titulo: Classes Abstratas e Interfaces
tipo: conceito
tags: [poo, classes-abstratas, interfaces, abstract, implements, heranca-multipla, java]
disciplina: Linguagens de Programação
fontes: [lp-a08-poo-linguagem-java]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Classes Abstratas e Interfaces

## Classes Abstratas

### Definição
Classe que serve **apenas como modelo estrutural** para subclasses; **não pode ser instanciada** diretamente. Define a estrutura (métodos abstratos) que todas as subclasses devem implementar.

### Características
- Declarada com `abstract class`
- Métodos abstratos (`abstract void nomeMetodo()`) não têm implementação — obrigatoriamente implementados nas subclasses
- Pode conter métodos concretos (com implementação) convivendo com abstratos
- Subclasse herda via `extends`

```java
public abstract class Profissao {
    public abstract void trabalhar();  // sem implementação
}

public class Agricultor extends Profissao {
    private void trabalhar() {
        System.out.println("Agricultor planta.");
    }
}
```

## Interfaces

### Definição
Tipo especial de classe abstrata: contém **apenas declarações de métodos** (sem implementação), além de atributos implicitamente `static` e `final`. Classes "assinam" a interface via `implements`.

### Características
- Declarada com `interface`
- Implementada por classes via `implements`
- `@Override` usado ao implementar os métodos
- Permite **herança múltipla**: uma classe pode implementar várias interfaces (`implements A, B`)
- Java 8+: métodos `default` em interfaces permitem implementação padrão opcional

```java
public interface Profissao {
    public void trabalhar();
}

public class Agricultor implements Profissao {
    @Override
    private void trabalhar() {
        System.out.println("Agricultor planta.");
    }
}
```

## Comparação

| | Classe Abstrata | Interface |
|--|----------------|-----------|
| Instanciável? | Não | Não |
| Pode ter implementação? | Sim (métodos concretos) | Só com `default` (Java 8+) |
| Herança múltipla? | Não (`extends` = 1 superclasse) | Sim (`implements A, B, C`) |
| Palavra-chave subclasse | `extends` | `implements` |
| Atributos | Qualquer tipo | `static` e `final` |

## Quando Usar Cada Um

- **Classe abstrata**: quando há lógica comum a todas as subclasses E uma hierarquia única de herança
- **Interface**: quando se quer definir um contrato que múltiplas classes não relacionadas devem seguir, ou quando herança múltipla é necessária

### Caso de uso clássico de interface:
Classes A, B, C herdam de Z. Apenas B e C devem ter um comportamento X. Se X fosse colocado em Z, A também herdaria. Solução: criar uma interface com X e associá-la apenas a B e C.

## Relações

- [Herança](heranca.md) — classes abstratas usam herança; interfaces contornam suas limitações
- [Polimorfismo](polimorfismo.md) — `@Override` é central no uso de interfaces e classes abstratas
- [Encapsulamento](encapsulamento.md) — modificadores de acesso se aplicam também a classes abstratas
- [Linguagem Java](linguagem-java.md) — fonte principal destes conceitos

## Fontes

- [LP A8 — POO: Linguagem Java](../fontes/lp-a08-poo-linguagem-java.md)
