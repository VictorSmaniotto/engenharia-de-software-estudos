---
titulo: Linguagem Go
tipo: conceito
tags: [go, golang, google, programacao-estruturada, concorrencia, threads, linguagens]
disciplina: Linguagens de Programação
fontes: [lp-a05-programacao-estruturada-outras-linguagens]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Linguagem Go

## Definição

Linguagem de propósito geral desenvolvida pela **Google**, baseada no C, criada para servir como ferramenta otimizada para seu sistema operacional Android. Rapidamente ganhou adeptos por sua simplicidade e características próprias.

## Características Principais

- Baseada em C: sintaxe semelhante, estruturas de controle reconhecíveis
- Propósito geral: pode ser usada como linguagem estruturada clássica ou explorar concorrência
- **Retorno múltiplo de funções**: uma função pode retornar mais de um valor — recurso ausente nas demais linguagens populares (C, Java, Python)

## Programação Concorrente

O principal diferencial do Go é o suporte nativo a **programação concorrente**:
- Programas separados ou **threads (goroutines)** executados paralelamente
- Paralelismo via divisão de tempo em um único processador, ou execução real em múltiplos núcleos/processadores
- Útil para sistemas de alto desempenho, servidores e aplicações Android

> Programação concorrente pode ser considerada um paradigma próprio, distinto do estruturado. (LP A5)

## Sintaxe

```go
package main          // nome do pacote (módulo)
import "fmt"          // importa biblioteca de E/S

func main() {
    var lista = [5]int{10, 20, 30, 40, 50}  // vetor com inicialização inline
    fmt.Println("Lista:", lista)

    for i := 0; i < 5; i++ {               // laço com variável embutida
        lista[i] = lista[i] / 2
    }
}
```

### Diferenças sintáticas em relação ao C

| Elemento | C | Go |
|----------|---|----|
| Biblioteca E/S | `#include <stdio.h>` | `import "fmt"` |
| Agrupamento de arquivos | — | `package nome` |
| Declaração de vetor | `int lista[5];` | `var lista = [5]int{...}` |
| Saída com nova linha | `printf("...\n")` | `fmt.Println(...)` |
| Retorno múltiplo | Não | Sim |

## Relações

- [Linguagem C](linguagem-c.md) — Go é baseada em C; sintaxe semelhante e otimizada
- [Paradigma Estruturado](paradigma-estruturado.md) — Go é estruturada por padrão
- [Vetores e Matrizes](vetores-e-matrizes.md) — Go tem vetores com sintaxe diferente do C

## Fontes

- [LP A5 — Programação Estruturada: Outras Linguagens](../fontes/lp-a05-programacao-estruturada-outras-linguagens.md)
