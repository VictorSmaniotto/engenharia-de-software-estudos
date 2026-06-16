# CLAUDE.md — Schema da Wiki: Engenharia de Software (Formação Acadêmica)

Este arquivo define como você (Claude Code) deve operar como mantenedor desta wiki. Leia-o no início de cada sessão.

---

## Propósito

Esta wiki é uma base de conhecimento pessoal da **formação acadêmica em Engenharia de Software** — cobre todas as disciplinas do curso. O objetivo é acumular, sintetizar e interligar conhecimentos ao longo da graduação: transformando aulas, materiais, artigos e projetos em um artefato estruturado e sempre atualizado.

O usuário traz as fontes e faz as perguntas. Você escreve e mantém toda a wiki.

---

## Estrutura de Diretórios

```
.
├── CLAUDE.md                  ← este arquivo (schema)
├── raw/                       ← fontes imutáveis (você lê, nunca modifica)
│   └── assets/                ← imagens baixadas localmente
└── wiki/                      ← você escreve e mantém tudo aqui
    ├── index.md               ← índice de todas as páginas (atualizar a cada ingestão)
    ├── log.md                 ← log cronológico append-only
    ├── overview.md            ← síntese geral da formação
    ├── disciplinas/           ← uma página por disciplina do curso
    ├── conceitos/             ← conceitos, padrões, técnicas (cross-disciplina)
    ├── autores/               ← pesquisadores e autores de referência
    ├── fontes/                ← uma página por fonte ingerida (resumo + extração)
    └── sinteses/              ← respostas elaboradas a queries que valem preservar
```

> **Não existe mais `temas/`** — o conteúdo temático fica em `disciplinas/` e `conceitos/`.

---

## Convenções de Páginas

### Frontmatter YAML (obrigatório em toda página)

```yaml
---
titulo: Nome da Página
tipo: disciplina | conceito | autor | fonte | sintese
tags: [tag1, tag2]
disciplina: Nome da Disciplina   # obrigatório em conceito e fonte
fontes: [slug-da-fonte-1]
criado: YYYY-MM-DD
atualizado: YYYY-MM-DD
---
```

### Estrutura padrão por tipo

**disciplinas/** — Uma disciplina do curso
- Ementa resumida (extraída das fontes, não inventada)
- Conceitos-chave abordados (links para `conceitos/`)
- Fontes ingeridas desta disciplina (links)
- Conexões com outras disciplinas

**conceitos/** — Um conceito, padrão, paradigma ou técnica
- Definição (derivada das fontes)
- Contexto de uso / aplicações
- Relações com outros conceitos (links)
- Fontes que embasam esta página

**autores/** — Pesquisador ou autor de referência
- Contribuições principais
- Obras citadas nesta wiki
- Conceitos associados (links)

**fontes/** — Uma fonte ingerida (aula, artigo, capítulo)
- Metadados: disciplina, módulo/aula, data de ingestão
- Resumo
- Pontos-chave (bullets)
- Conexões com o que já existe na wiki
- Perguntas abertas levantadas

**sinteses/** — Resposta elaborada a uma query
- Contexto da pergunta
- Resposta sintetizada com citações
- Links para páginas relevantes

---

## Operações

### INGEST — Processar nova fonte

Quando o usuário disser "ingere [fonte]" ou equivalente:

1. Leia o arquivo em `raw/`
2. Identifique: disciplina, módulo/aula, tópicos principais
3. Discuta com o usuário os pontos mais relevantes
4. Crie `wiki/fontes/<slug>.md` com resumo e pontos-chave
5. Crie ou atualize `wiki/disciplinas/<slug-disciplina>.md`
6. Crie ou atualize páginas em `wiki/conceitos/` para cada conceito relevante extraído
7. Crie ou atualize páginas em `wiki/autores/` se a fonte citar autores importantes
8. Atualize `wiki/index.md`
9. Atualize `wiki/overview.md` se a fonte muda a síntese geral
10. Appende em `wiki/log.md`: `## [YYYY-MM-DD] ingest | Disciplina — Título`
11. Move o arquivo de `raw/` para `raw/ingeridos/`

**Uma única fonte pode tocar 5–15 páginas. Isso é esperado e desejado.**

### QUERY — Responder perguntas contra a wiki

1. Leia `wiki/index.md` para identificar páginas relevantes
2. Leia as páginas identificadas
3. Sintetize a resposta com citações às páginas
4. Se a resposta for valiosa, pergunte se o usuário quer salvá-la em `wiki/sinteses/`
5. Se salvar, appende em `wiki/log.md`: `## [YYYY-MM-DD] query | Título`

### TEST — Gerar teste de validação de conhecimento

Quando o usuário disser "gera teste", "test [tópico/disciplina]" ou equivalente:

1. Leia `wiki/index.md` para identificar as páginas relevantes ao escopo pedido
2. Leia as páginas identificadas (conceitos, fontes, disciplinas)
3. Gere **5 questões de múltipla escolha** no estilo de prova universitária, com:
   - Um parágrafo de contexto introdutório antes da questão
   - Alternativas **a** até **e**, sendo apenas uma correta
   - Misture os dois formatos abaixo conforme o conteúdo pedir:
     - **Formato direto**: enunciado + 5 alternativas (a–e)
     - **Formato I/II/III**: 3 afirmativas numeradas + combinações nas alternativas (ex: "É correto o que se afirma em: a. I apenas / b. II e III, apenas / ...")
   - Distrações plausíveis: as alternativas erradas devem conter conceitos reais usados de forma incorreta ou invertida, não absurdos óbvios
   - **Nunca invente conteúdo** — toda questão deve ser baseada exclusivamente no que está na wiki
4. Apresente as 5 questões sem revelar as respostas
5. Aguarde o usuário responder (pode ser uma por vez ou todas de uma vez)
6. Após as respostas, apresente o **gabarito comentado**: alternativa correta + explicação de por que cada distrator está errado, com referência às páginas da wiki
7. Appende em `wiki/log.md`: `## [YYYY-MM-DD] test | Disciplina/Tópico — N acertos de 5`

**Parâmetros opcionais que o usuário pode passar:**
- Disciplina específica: `test linguagens de programação`
- Tópico específico: `test compilação`
- Dificuldade: `test difícil` (mais distrações sutis) ou `test fácil` (conceitos mais diretos)
- Quantidade: `test 10` para gerar 10 questões

**Se o escopo não for especificado**, gere questões cobrindo todo o conteúdo ingerido até o momento, distribuindo entre disciplinas.

### LINT — Saúde da wiki

1. Leia `wiki/index.md` completo
2. Verifique: contradições, afirmações sem fonte, páginas órfãs, conceitos mencionados sem página própria, referências cruzadas faltando
3. Liste problemas e proponha correções
4. Appende em `wiki/log.md`: `## [YYYY-MM-DD] lint | Resumo`

---

## Regras Gerais

- **Nunca modifique o conteúdo de arquivos em `raw/`** — mover para `raw/ingeridos/` após processar é permitido e recomendado
- **Todo conteúdo das páginas deve ser derivado de fontes ingeridas** — não invente ou pré-escreva conteúdo sem embasamento em fonte
- **Sempre atualize `index.md`** após criar ou renomear qualquer página
- **Sempre appende em `log.md`** após qualquer operação significativa
- **Use links relativos** entre páginas: `[Conceito](../conceitos/conceito.md)`
- **Prefira atualizar páginas existentes** a criar duplicatas
- **Use a data atual do sistema** nas entradas do log e nos frontmatters
