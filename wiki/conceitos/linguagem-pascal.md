---
titulo: Linguagem Pascal (e Delphi)
tipo: conceito
tags: [pascal, delphi, programacao-estruturada, gui, linguagens]
disciplina: Linguagens de Programação
fontes: [lp-a05-programacao-estruturada-outras-linguagens]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Linguagem Pascal (e Delphi)

## Pascal

Linguagem estruturada com sintaxe legível e próxima do C, mas com notação própria. Usada historicamente como linguagem de ensino pela clareza de código.

### Diferenças sintáticas em relação ao C

| Elemento | C | Pascal |
|----------|---|--------|
| Bloco de comandos | `{ }` | `begin ... end` |
| Atribuição | `=` | `:=` |
| Delimitador de texto | `"aspas"` | `'apóstrofos'` |
| E/S de dados | `printf` / `scanf` (biblioteca) | `writeln` / `readln` (palavra reservada) |
| Importar biblioteca | `#include` | `uses` (após nome do programa) |
| Laço contado | `for (i=0; i<n; i++)` | `for i := 1 to n do` |
| Declaração de variáveis | inline | bloco `var` antes do `begin` |

### Estrutura básica

```pascal
program NomePrograma;
uses NomeBiblioteca;
var
  a, b: integer;
begin
  { código aqui }
end.
```

## Delphi

Evolução comercial do Pascal para desenvolvimento de **software com interface gráfica (GUI)**.

- Componentes visuais (botões, campos, seletores) criados graficamente e tratados como **objetos**
- Cada componente tem propriedades: tamanho, cor, nome, dado armazenado, etc.
- Palavra reservada `procedure` gerencia janelas e os eventos de seus componentes
- Lógica do código interno (atribuições, estruturas de controle) permanece igual ao Pascal
- Perdeu espaço para Java, C e Python, mas mantém sistemas legados ativos até hoje

> A transição Pascal → Delphi demonstra que conhecer a linguagem-base facilita a adaptação a suas evoluções. (LP A5)

## Relações

- [Linguagem C](linguagem-c.md) — Pascal e C são contemporâneos e compartilham a base estruturada
- [Paradigma Estruturado](paradigma-estruturado.md) — Pascal é exemplo representativo
- [Paradigma OO](paradigma-oo.md) — Delphi antecipa conceitos de OO (componentes como objetos) sem ser formalmente OO

## Fontes

- [LP A5 — Programação Estruturada: Outras Linguagens](../fontes/lp-a05-programacao-estruturada-outras-linguagens.md)
