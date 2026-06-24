---
titulo: "ALP Aula 16 — Manipulação de Arquivos de Texto"
tipo: fonte
tags: [arquivo, persistencia, crud, texto, forbellone, fda]
disciplina: Algoritmos e Lógica de Programação
fontes: [alp-aula16-manipulacao-arquivos]
criado: 2026-06-15
atualizado: 2026-06-15
---

# ALP Aula 16 — Manipulação de Arquivos de Texto

**Disciplina:** Algoritmos e Lógica de Programação  
**Módulo/Aula:** Aula 16  
**Data de ingestão:** 2026-06-15

---

## Resumo

Introduz o conceito de **persistência de dados** via arquivos de texto. Dados em variáveis são perdidos ao término de um algoritmo; arquivos permitem que dados sobrevivam entre execuções. Apresenta as palavras reservadas para manipulação de arquivos segundo Forbellone (2005).

---

## Pontos-chave

- **Problema da efemeridade:** dados em memória (variáveis, vetores, registros) são perdidos ao fim da execução; arquivos de texto ou binários oferecem permanência.
- **Foco em arquivos de texto:** arquivos binários são mais complexos; a aula concentra-se nos de texto (caracteres), que suportam grandes volumes de dados em tamanho reduzido.
- **CRUD:** Create, Read, Update, Delete — operações básicas de gerenciamento de dados, válidas tanto para arquivos quanto para bancos de dados.
- **Declaração de tipo arquivo:**
  ```
  TIPO CADASTRO = REGISTRO
    INTEIRO: CODIGO, IDADE;
    CARACTERE: NOME, ENDERECO, CIDADE, ESTADO
  FIMREGISTRO;
  TIPO ARQ = ARQUIVO COMPOSTO DE CADASTRO;
  CADASTRO: DADOS;
  ARQ: AGENDA;
  ```
- **Palavras reservadas (Forbellone, 2005):**
  | Instrução | Ação |
  |-----------|------|
  | `ABRA(ARQ)` | Abre o arquivo para uso |
  | `AVANCE(ARQ)` | Move índice para a próxima linha |
  | `GUARDE(ARQ, VAR)` | Grava o conteúdo da variável na próxima linha |
  | `COPIE(ARQ, VAR)` | Lê a linha atual para a variável |
  | `FECHE(ARQ)` | Fecha o arquivo (garante integridade) |
  | `ELIMINE(ARQ)` | Exclui o arquivo inteiro (irreversível) |
  | `FDA(ARQ)` | Condição "fim de arquivo"; usada com `ATÉ` para controlar laço de leitura |
- **Padrão de inserção:** `ABRA` → laço com `AVANCE/ATÉ FDA` para chegar ao final → `LEIA` dos campos → `GUARDE` → `FECHE`.
- **Padrão de leitura:** `ABRA` → laço `REPITA/AVANCE/COPIE/ATÉ FDA` carregando dados em vetor de registros → processar → `FECHE`.
- **Organização de dados:** sem estrutura obrigatória no arquivo; o desenvolvedor define separadores (ex.: `#`) entre campos na mesma linha para simular registros.

---

## Conceitos relacionados

- [Manipulação de Arquivos](../conceitos/manipulacao-de-arquivos.md)
- [Registro](../conceitos/registro.md)
- [Vetores e Matrizes](../conceitos/vetores-e-matrizes.md)
- [Estruturas de Repetição](../conceitos/estruturas-de-repeticao.md)

---

## Perguntas abertas

- Como o conceito de `ARQUIVO COMPOSTO DE REGISTRO` se relaciona com tabelas em SQL?
- O que é `FDA` em termos de implementação? Equivale ao EOF (End of File) de linguagens como C?
