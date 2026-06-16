# Wiki — Engenharia de Software (Formação Acadêmica)

Base de conhecimento pessoal mantida pelo Claude Code. Cobre todas as disciplinas do curso.

## Como usar

**Ingerir uma aula:** coloque o arquivo em `raw/` e diga _"ingere [arquivo]"_.

**Fazer uma pergunta:** pergunte diretamente. O Claude consulta a wiki e responde com citações.

**Lint:** diga _"faz um lint da wiki"_ para checar saúde do conteúdo.

---

## Estrutura

```
raw/               ← seus arquivos de aula (nunca modificados)
wiki/
  index.md         ← índice de tudo
  log.md           ← histórico de operações
  overview.md      ← síntese geral da formação
  disciplinas/     ← uma página por disciplina
  conceitos/       ← conceitos e paradigmas (cross-disciplina)
  autores/         ← autores de referência
  fontes/          ← resumos das fontes ingeridas
  sinteses/        ← respostas elaboradas salvas
CLAUDE.md          ← schema (instruções para o Claude)
```
