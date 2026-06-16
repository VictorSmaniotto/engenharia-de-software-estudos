---
titulo: Manipulação de Arquivos de Texto
tipo: conceito
tags: [arquivo, persistencia, crud, fda, forbellone, texto]
disciplina: Algoritmo e Lógica de Programação
fontes: [alp-aula16-manipulacao-arquivos]
criado: 2026-06-15
atualizado: 2026-06-15
---

# Manipulação de Arquivos de Texto

## Definição

Arquivos de texto permitem **persistência de dados** além do tempo de execução de um algoritmo. Dados armazenados em variáveis em memória são perdidos ao término da execução; arquivos em disco permanecem disponíveis para execuções futuras.

## Declaração de Tipo Arquivo

O tipo arquivo é declarado a partir de um registro existente:

```
TIPO CADASTRO = REGISTRO
  INTEIRO: CODIGO, IDADE;
  CARACTERE: NOME, ENDERECO
FIMREGISTRO;

TIPO ARQ = ARQUIVO COMPOSTO DE CADASTRO;

CADASTRO: DADOS;   ← variável para manipulação em memória
ARQ: AGENDA;       ← variável para manipulação do arquivo
```

## Palavras Reservadas (Forbellone, 2005)

| Instrução | Ação |
|-----------|------|
| `ABRA(AGENDA)` | Abre o arquivo para uso |
| `AVANCE(AGENDA)` | Move o índice para a próxima linha do arquivo |
| `GUARDE(AGENDA, DADOS)` | Grava o conteúdo de `DADOS` na próxima linha |
| `COPIE(AGENDA, DADOS)` | Lê a linha atual do arquivo para `DADOS` |
| `FECHE(AGENDA)` | Fecha o arquivo (protege integridade) |
| `ELIMINE(AGENDA)` | Exclui o arquivo inteiro (irreversível) |
| `FDA(AGENDA)` | Condição booleana: verdadeira ao atingir o fim do arquivo |

## Padrão de Inserção

```
ABRA (AGENDA);
REPITA
  AVANCE (AGENDA);
ATÉ FDA (AGENDA);
LEIA (REGISTRO.NOME);
LEIA (REGISTRO.TELEFONE);
GUARDE (AGENDA, REGISTRO);
FECHE (AGENDA);
```

## Padrão de Leitura para Vetor

```
ABRA (AGENDA);
REPITA
  AVANCE (AGENDA);
  COPIE (AGENDA, LISTA[I]);
  I <- I + 1;
ATÉ FDA (AGENDA);
```

## CRUD

As operações básicas de gerenciamento de dados em qualquer contexto (arquivo ou banco):
- **Create** — inserir novo registro (`GUARDE`)
- **Read** — ler registro (`COPIE`)
- **Update** — ler, modificar, regravar
- **Delete** — usar `ELIMINE` com cuidado (apaga o arquivo todo)

## Observações

- Arquivos de texto não têm estrutura obrigatória; o desenvolvedor define separadores (ex.: `#`) para organizar campos em cada linha.
- `FECHE` deve sempre ser chamado para garantir que dados em buffer sejam gravados e o arquivo não fique corrompido.
- `ELIMINE` é irreversível — usar com máxima cautela.

## Relações

- [Registro](registro.md)
- [Vetores e Matrizes](vetores-e-matrizes.md)
- [Estruturas de Repetição](estruturas-de-repeticao.md)
