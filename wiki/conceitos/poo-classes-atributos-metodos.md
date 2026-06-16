---
titulo: "POO: Classes, Atributos, Métodos e Objetos"
tipo: conceito
tags: [poo, classes, atributos, metodos, objetos, construtor, abstracao]
disciplina: Linguagens de Programação
fontes: [lp-a06-poo-conceitos]
criado: 2026-05-11
atualizado: 2026-05-11
---

# POO: Classes, Atributos, Métodos e Objetos

## Os Quatro Elementos Centrais do OO

| Elemento | Papel | Analogia estruturada |
|----------|-------|----------------------|
| **Classe** | Modelo/template que define estrutura e comportamentos | Registro (`struct`) + sub-rotinas |
| **Atributo** | Propriedade da classe; armazena dados do objeto | Campo do registro |
| **Método** | Sub-rotina pertencente à classe; processa atributos | Função/procedimento |
| **Objeto** | Instância particular da classe; tem seus próprios valores | Variável do tipo registro |

## Classe

- Define quais atributos existem e quais métodos podem ser executados
- **Não armazena dados em si** — é apenas o molde
- Uma única classe pode gerar inúmeros objetos, cada um com dados independentes
- Evolução dos registros (`struct`) do paradigma estruturado: integra dados e comportamentos

## Atributo

- Equivale a campo de um registro, mas dentro de uma classe
- Tem tipo de dado definido (int, float, char, boolean, etc.)
- Cada objeto instanciado da classe possui seus próprios valores para os atributos
- Normalmente declarado como `private` (encapsulamento) — acessível só pelos métodos da classe

## Método

- Equivale a sub-rotinas; processa e manipula os atributos da classe
- Declarado dentro da classe; tem acesso direto aos atributos
- **set()**: recebe e armazena dados em um atributo (entrada)
- **get()**: retorna o valor de um atributo (saída)
- Podem ser criados métodos específicos para funcionalidades além do set/get básico

### Construtor e Destrutor

| Método | Nome | Quando executado | Finalidade |
|--------|------|-----------------|-----------|
| **Construtor** | Mesmo nome da classe | Ao instanciar o objeto | Inicializa atributos; evita lixo de memória |
| **Destrutor** | `~NomeDaClasse()` | Ao encerrar o uso do objeto | Libera recursos de hardware alocados |

## Objeto

- Instância concreta de uma classe com dados próprios
- Criado por instanciação: `NomeDaClasse obj = new NomeDaClasse();` (Java)
- Métodos são chamados via o objeto: `obj.nomeMetodo()`
- Atributos de um objeto são independentes dos atributos de outro objeto da mesma classe

## Abstração como Ponto de Partida

Para modelar classes a partir de um problema real:
1. Compreender o **escopo do problema** (o que o software precisa resolver)
2. Identificar as **entidades relevantes** (animais, clientes, produtos, etc.)
3. Para cada entidade: definir **atributos** (características necessárias) e **métodos** (ações necessárias)
4. Separar entidades distintas em classes distintas (ex: não misturar dados do animal com dados do dono)

## Relações

- [Paradigma OO](paradigma-oo.md) — visão geral do paradigma
- [Encapsulamento](encapsulamento.md) — controla visibilidade de atributos e métodos
- [Herança](heranca.md) — permite que subclasses herdem atributos e métodos
- [Linguagem Java](linguagem-java.md) — implementação concreta destes conceitos
- [Linguagem C](linguagem-c.md) — `struct` é o precursor direto das classes
- [Escopo](escopo.md) — variáveis de métodos têm escopo local; atributos pertencem ao objeto

## Fontes

- [LP A6 — POO: Conceitos de Classes, Atributos, Métodos e Objetos](../fontes/lp-a06-poo-conceitos.md)
