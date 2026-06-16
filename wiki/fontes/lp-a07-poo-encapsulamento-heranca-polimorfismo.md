---
titulo: "LP A7 — POO: Encapsulamento, Herança e Polimorfismo"
tipo: fonte
tags: [poo, encapsulamento, heranca, polimorfismo, superclasse, subclasse, modificadores-de-acesso]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-11
atualizado: 2026-05-11
---

# LP A7 — POO: Encapsulamento, Herança e Polimorfismo

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Linguagens de Programação |
| Aula | 7 |
| Fonte original | https://ead.unimar.br/aulas/linguagens-de-programacao/aula-07.html |
| Data de ingestão | 2026-05-11 |

---

## Resumo

Apresenta os três pilares diferenciais do paradigma OO em relação ao estruturado: encapsulamento (controle de visibilidade), herança (reutilização e extensão de classes) e polimorfismo (personalização de métodos em subclasses). Detalha os modificadores de acesso `private`, `public` e `protected` e sua relação com a herança.

---

## Pontos-chave

### Encapsulamento
- Empacotamento de atributos e métodos dentro de uma classe, tornando-a independente e segura
- Garante que dados sejam processados de forma controlada → software mais confiável
- Três **modificadores de acesso**:

| Modificador | Visibilidade |
|-------------|-------------|
| `private` | Apenas dentro da própria classe; invisível às demais |
| `public` | Visível por qualquer classe do mesmo pacote/software |
| `protected` | Visível apenas por subclasses via herança |

- Classes são sempre `public` (único ponto de acesso a seus internos)
- Atributos devem ser preferencialmente `private` para segurança
- Uso de `public` em atributos reduz encapsulamento e aumenta exposição do software

### Herança
- Permite que uma **subclasse** herde atributos e métodos de uma **superclasse**
- Terminologia equivalente: superclasse = classe pai/mãe; subclasse = classe filha
- Objetivo: reduzir redundância de código e estruturar a modelagem de forma coerente
- Superclasse define atributos e métodos gerais (ex: Veículos, Animais, Atividade)
- Subclasses estendem com especificidades (ex: Utilitários, Mamíferos, Comércio)
- Subclasses não são totalmente dependentes da superclasse — usam herança quando conveniente
- Atributos/métodos `protected` na superclasse são acessíveis pelas subclasses

### Polimorfismo
- Complemento da herança: permite que uma subclasse **reescreva** um método da superclasse com o mesmo nome
- Uso: quando a superclasse define um método que a subclasse necessita, mas com comportamento diferente
- Exemplo: método `locomover()` em Animais; Mamíferos andam e nadam, Peixes só nadam → cada subclasse implementa sua versão
- Resultado: classes interligadas mantêm suas particularidades sem conflito com a herança

### Linguagens e Suporte a OO
- **Só estruturado** (sem OO): C, Pascal
- **OO opcional** (estruturado + OO): C++, C#, Objective-C, Python, PHP, JavaScript
- **OO obrigatório** (só OO): Java, Objective-C (em certos contextos)

---

## Conexões com o que já existe na wiki

- [Paradigma OO](../conceitos/paradigma-oo.md): esta aula detalha os três pilares do paradigma
- [Linguagem Java](../conceitos/linguagem-java.md): exemplo prático dos três conceitos em Java
- [Linguagem C](../conceitos/linguagem-c.md): referência como linguagem sem suporte a OO
- [Paradigma Estruturado](../conceitos/paradigma-estruturado.md): OO é uma evolução/alternativa ao estruturado

---

## Perguntas abertas

- Em quais situações o polimorfismo é preferível a simplesmente criar métodos com nomes diferentes?
- O uso de `protected` é sempre a melhor escolha quando há herança, ou existem exceções?
