---
titulo: Polimorfismo
tipo: conceito
tags: [poo, polimorfismo, override, heranca, subclasse, metodos]
disciplina: Linguagens de Programação
fontes: [lp-a07-poo-encapsulamento-heranca-polimorfismo, lp-a08-poo-linguagem-java]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Polimorfismo

## Definição

Mecanismo do paradigma OO que permite que uma **subclasse reescreva um método da superclasse com o mesmo nome**, adaptando seu comportamento às especificidades da subclasse, sem quebrar o vínculo da herança.

> "O polimorfismo permite que uma subclasse reescreva métodos de uma superclasse usando o mesmo nome e assim, podendo personalizar este método para seu uso." (LP A7)

## Por que Usar

Quando a superclasse define um método genérico que faz sentido para todas as subclasses, mas cada subclasse tem uma variação específica:

- Superclasse `Animais` tem método `locomover()` → todos os animais se locomovem
- `Mamíferos`: andam e nadam
- `Peixes`: apenas nadam

Sem polimorfismo, seria necessário criar métodos com nomes diferentes em cada subclasse, perdendo a coerência da hierarquia.

## Em Java: `@Override`

```java
public class Profissao {
    protected void trabalhar() {
        System.out.println("Profissional trabalha.");
    }
}

public class Agricultor extends Profissao {
    @Override
    private void trabalhar() {
        System.out.println("Agricultor planta.");
    }
}

public class Pedreiro extends Profissao {
    @Override
    private void trabalhar() {
        System.out.println("Pedreiro constrói.");
    }
}
```

- `@Override`: informa ao compilador que o método sobrescreve um de mesmo nome na superclasse
- Se o nome não existir na superclasse → **erro de compilação** (auxilia manutenção de código)
- Protege contra renomeações acidentais de métodos em hierarquias grandes

## Relações

- [Herança](heranca.md) — polimorfismo é o complemento natural da herança
- [Encapsulamento](encapsulamento.md) — modificadores de acesso determinam o que pode ser sobrescrito
- [Classes Abstratas e Interfaces](classes-abstratas-interfaces.md) — polimorfismo é central no uso de abstrações
- [Linguagem Java](linguagem-java.md) — `@Override` é a anotação de polimorfismo em Java

## Fontes

- [LP A7 — POO: Encapsulamento, Herança e Polimorfismo](../fontes/lp-a07-poo-encapsulamento-heranca-polimorfismo.md)
- [LP A8 — POO: Linguagem Java](../fontes/lp-a08-poo-linguagem-java.md)
