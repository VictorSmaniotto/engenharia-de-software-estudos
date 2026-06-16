---
titulo: Linguagem PHP
tipo: conceito
tags: [php, web, back-end, front-end, html, programacao-estruturada, linguagens]
disciplina: Linguagens de Programação
fontes: [lp-a05-programacao-estruturada-outras-linguagens]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Linguagem PHP

## Definição

Linguagem de programação originalmente estruturada, voltada para o desenvolvimento **web no servidor (back-end)**. Interpretada pelo servidor; o resultado é enviado ao navegador do usuário.

## PHP + HTML: Front-end e Back-end

| Camada | Tecnologia | Responsabilidade |
|--------|-----------|-----------------|
| **Front-end** | HTML | Estrutura da página: textos, imagens, formulários, elementos visuais |
| **Back-end** | PHP | Acesso a banco de dados, processamento de dados, lógica de negócio |

As duas linguagens se complementam para criar sistemas web interativos (equivalente funcional de sistemas desktop como Delphi).

## Características da Linguagem

- Baseada em C: estruturas de controle (`if`, `while`, `for`) idênticas ao C
- **`$` antes de todo nome de variável**: facilita identificação em meio ao HTML
- Scripts PHP embutidos em HTML via delimitadores `<?php ... ?>`
- Aceita tags HTML dentro do PHP (ex: `echo "</br>"` para quebra de linha)
- Suporta também **programação orientada a objetos** além do estilo estruturado

## Estrutura básica

```php
<!DOCTYPE html>
<html>
<body>
  <h1>Título</h1>
  <?php
    $variavel = "valor";
    echo $variavel;
  ?>
</body>
</html>
```

## Relações

- [Linguagem C](linguagem-c.md) — PHP deriva sintaticamente do C
- [Paradigma Estruturado](paradigma-estruturado.md) — PHP é exemplo de linguagem estruturada com ampla adoção comercial
- [Paradigma OO](paradigma-oo.md) — PHP também suporta OO opcionalmente

## Fontes

- [LP A5 — Programação Estruturada: Outras Linguagens](../fontes/lp-a05-programacao-estruturada-outras-linguagens.md)
