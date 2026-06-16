---
titulo: "LP A5 — Programação Estruturada: Outras Linguagens"
tipo: fonte
tags: [pascal, delphi, php, go, programacao-estruturada, linguagens]
disciplina: Linguagens de Programação
fontes: []
criado: 2026-05-11
atualizado: 2026-05-11
---

# LP A5 — Programação Estruturada: Outras Linguagens

## Metadados

| Campo | Valor |
|-------|-------|
| Disciplina | Linguagens de Programação |
| Aula | 5 |
| Fonte original | https://ead.unimar.br/aulas/linguagens-de-programacao/aula-05.html |
| Data de ingestão | 2026-05-11 |

---

## Resumo

Apresenta quatro linguagens além do C que também se baseiam na programação estruturada: Pascal, Delphi (evolução de Pascal para GUIs), PHP (web) e GO (Google, concorrência). Reforça que linguagens diferentes compartilham aspectos sintáticos oriundos do C, facilitando o aprendizado cruzado.

---

## Pontos-chave

### Pascal
- Sintaxe semelhante ao C, mas com diferenças notáveis de notação
- `begin` / `end` como delimitadores de bloco (em vez de `{ }`)
- Atribuição com `:=` (em vez de `=`)
- Texto delimitado por apóstrofos `'` (em vez de aspas)
- `readln()` / `writeln()` são palavras reservadas da própria linguagem (não de biblioteca)
- Estrutura `for i := 1 to n do` para laço contado
- Bibliotecas incluídas via palavra reservada `uses` (logo após a nomeação do programa)
- Variáveis declaradas em bloco `var` antes do `begin`
- Boas práticas: inicializar variáveis antes do primeiro uso para evitar lixo de memória

### Delphi
- Evolução comercial do Pascal para desenvolvimento de software com **interface gráfica (GUI)**
- Componentes visuais (botões, campos, seletores) criados graficamente e nomeados como objetos
- Cada componente vira um objeto com propriedades (tamanho, cor, nome, dado armazenado)
- Palavra reservada `procedure` gerencia janelas e ações de componentes
- Lógica do código em si mantém a base Pascal; apenas a camada de componentes é diferente
- Perdeu mercado para Java, C e Python; mas possui sistemas legados ainda ativos

### PHP
- Linguagem originalmente estruturada, voltada para **desenvolvimento web (back-end)**
- Interpretada pelo servidor web; HTML é o front-end; PHP é o back-end
- **Front-end** (HTML): estrutura da página — textos, imagens, formulários
- **Back-end** (PHP): acesso a bancos de dados, processamento de dados, lógica do sistema
- Baseada em C: estruturas de controle iguais; diferencial: `$` antes de todo nome de variável
- Scripts PHP embutidos em HTML via delimitadores `<?php ... ?>`
- Tags HTML podem ser usadas dentro de PHP (ex: `echo "</br>"`)
- Aceita também orientação a objetos além do estruturado

### GO
- Desenvolvida pela **Google** para o SO Android; de propósito geral, baseada em C
- Característica principal: suporte nativo a **programação concorrente** (threads/goroutines)
- Concorrência: tarefas executadas "ao mesmo tempo" por divisão de tempo de processamento ou múltiplos núcleos/processadores
- Pode ser usada como linguagem puramente estruturada (concorrência é opcional)
- Diferencial único: função pode **retornar mais de um valor** (recurso ausente em C, Java, etc.)
- `package main`: agrupa arquivos de um mesmo software (modularidade)
- `import "fmt"`: importa biblioteca de entrada/saída
- Declaração de vetor: `var lista = [5]int{10,20,30,40,50}` (inicialização inline)
- Laço `for` com variável embutida: `for i:= 0; i < 5; i++ { ... }`

---

## Conexões com o que já existe na wiki

- Complementa [Linguagem C](../conceitos/linguagem-c.md): Pascal, PHP e GO derivam do C
- Confirma [Paradigma Estruturado](../conceitos/paradigma-estruturado.md): todas as linguagens usam a mesma base
- PHP e HTML: relaciona programação estruturada com paradigma declarativo
- GO introduz **programação concorrente** — novo paradigma a registrar futuramente
- Delphi antecipa conceitos de OO (componentes como objetos) sem ser formalmente OO

---

## Perguntas abertas

- Como a programação concorrente se classifica em relação ao framework de paradigmas de Sebesta?
- PHP também suporta OO — quando usar o estilo estruturado vs. orientado a objetos em PHP?
