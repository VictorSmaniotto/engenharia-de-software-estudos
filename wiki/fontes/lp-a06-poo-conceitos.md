---
titulo: "LP A6 — POO: Conceitos de Classes, Atributos, Métodos e Objetos"
tipo: fonte
tags: [poo, classes, atributos, metodos, objetos, abstracao, construtor]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-11
atualizado: 2026-05-11
---

# LP A6 — POO: Conceitos de Classes, Atributos, Métodos e Objetos

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Linguagens de Programação |
| Aula | 6 |
| Fonte original | https://ead.unimar.br/aulas/linguagens-de-programacao/aula-06.html |
| Data de ingestão | 2026-05-11 |

---

## Resumo

Introduz o paradigma orientado a objetos a partir da ideia de abstração: problemas reais são modelados em classes com atributos e métodos, das quais objetos são instanciados. Contrasta com a programação estruturada por meio da evolução de registros (struct) para classes. Apresenta os quatro elementos centrais do paradigma: classe, atributo, método e objeto.

---

## Pontos-chave

### Abstração
- Ponto de partida do OO: identificar as partes relevantes de um problema real e representá-las como estruturas de dados e comportamentos
- Processo: compreender o **escopo do problema** → identificar entidades → definir atributos e métodos necessários

### Evolução: Registro → Classe
- Na programação estruturada: **registro** (`struct` em C) agrupa campos de tipos diferentes — é um tipo definido pelo usuário
- Um registro vinculado a uma variável armazena uma ocorrência; vinculado a vetor, armazena múltiplas ocorrências
- No OO: **classe** substitui e evolui o registro — agrupa atributos (equivalentes a campos) E métodos (equivalentes a sub-rotinas), tornando dados e comportamentos inseparáveis

### Quatro Elementos do OO

| Elemento | Definição |
|----------|-----------|
| **Classe** | Modelo/template que define atributos e métodos; não armazena dados em si |
| **Atributo** | Propriedade definida na classe; armazena dados em cada objeto; equivale a campo do registro |
| **Método** | Sub-rotina dentro da classe; realiza processamento dos atributos |
| **Objeto** | Instância particular de uma classe; armazena um conjunto único de dados nos atributos |

### Relação entre Classe e Objeto
- Uma classe pode gerar **inúmeros objetos**, cada um com seus próprios valores de atributos
- Objetos são criados por **instanciação** da classe
- A classe é o molde; o objeto é o produto

### Métodos set() e get()
- **set()**: recebe e armazena dados em atributos (entrada)
- **get()**: retorna dados dos atributos (saída)
- Nomenclatura padrão; métodos mais específicos podem ser criados conforme o problema

### Construtor e Destrutor
- **Método construtor**: mesmo nome da classe; executado automaticamente na instanciação; inicializa atributos com valores adequados (evita lixo de memória)
- **Destrutor** (`~NomeClasse()`): executado ao finalizar o uso do objeto; libera recursos de hardware alocados

### Execução de Métodos em Memória
- Cada método em execução ocupa um espaço na memória com suas estruturas de dados
- Ao chamar outro método: estado do método chamador é pausado; novo espaço alocado para o chamado
- Ao encerrar o método chamado: retorno de dados ao chamador; memória liberada
- Ao encerrar o chamador: memória também liberada → ciclo contínuo durante a execução do software

---

## Conexões com o que já existe na wiki

- [Paradigma OO](../conceitos/paradigma-oo.md): esta aula fundamenta e detalha o paradigma já registrado
- [Linguagem C](../conceitos/linguagem-c.md): `struct` é o precursor direto das classes
- [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md): vetores de registros são precursores de coleções de objetos
- [Escopo](../conceitos/escopo.md): ciclo de vida de variáveis em métodos segue o mesmo princípio do estruturado

---

## Perguntas abertas

- Em quais situações convém usar métodos específicos em vez de apenas set/get genéricos?
- Como registros (`struct`) em C se relacionam com `struct` em linguagens OO como C++/Go?
