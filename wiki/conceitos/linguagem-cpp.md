---
titulo: Linguagem C++
tipo: conceito
tags: [cpp, multiparadigma, poo, estruturado, construtor, destrutor]
disciplina: Linguagens de Programação
fontes: [lp-a09-poo-outras-linguagens]
criado: 2026-05-19
atualizado: 2026-05-19
---

# Linguagem C++

## Definição

C++ é a extensão da linguagem C que adicionou o paradigma orientado a objetos ao estruturado, tornando-se uma **linguagem multiparadigma** (estruturado + OO). Mantém toda a compatibilidade com C e adiciona classes, encapsulamento, herança e polimorfismo.

## Características principais

- Superconjunto do C: todo código C válido compila em C++
- **Multiparadigma**: estruturado + OO (e moderno: também funcional a partir do C++11)
- Modificadores de acesso iguais ao Java: `public`, `protected`, `private`
- Suporta **encapsulamento, herança e polimorfismo**

## Organização de arquivos

C++ separa definição de implementação em dois arquivos:

| Arquivo | Conteúdo |
|---------|----------|
| `.hpp` (ou `.h`) | **Cabeçalho** — define a classe, atributos e assinaturas dos métodos |
| `.cpp` | **Implementação** — contém o código dos métodos |

O arquivo de implementação inclui o cabeçalho via `#include "animal.hpp"`, e ambos são compilados juntos para gerar o executável.

## Construtores e Destrutores

- **Construtor**: método com o **mesmo nome da classe**, sem tipo de retorno; inicializa atributos; chamado via `new` ou na instanciação direta do objeto
  - Uma classe pode ter vários construtores (sobrecarga)
- **Destrutor**: prefixo `~` antes do nome da classe; chamado quando o objeto não é mais necessário; libera recursos

```cpp
class Animal {
    int codigoAnimal;
public:
    void Animal(void) { codigoAnimal = 0; }   // construtor
    void ~Animal(void) { /* libera recursos */ }  // destrutor
};
```

## C# — Variação nos modificadores

A linguagem C# (Microsoft) estende os modificadores além do padrão C++/Java:
- `public`, `protected`, `private` (padrão)
- `internal` — acesso somente dentro do mesmo assembly
- `internal protected`
- `protected private`

## Relações

- [Linguagem C](linguagem-c.md) — base do C++
- [Paradigma Estruturado](paradigma-estruturado.md) — herdado do C
- [Paradigma OO](paradigma-oo.md) — adicionado ao C
- [Encapsulamento](encapsulamento.md) — public/protected/private
- [Herança](heranca.md) — suportada em C++
- [Polimorfismo](polimorfismo.md) — suportado em C++
- [POO: Classes, Atributos, Métodos e Objetos](poo-classes-atributos-metodos.md) — construtores/destrutores

## Fontes

- [LP A9 — POO: Outras Linguagens](../fontes/lp-a09-poo-outras-linguagens.md)
