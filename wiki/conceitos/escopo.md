---
titulo: Escopo de Variáveis
tipo: conceito
tags: [escopo, variaveis, funcoes, linguagem-c, memoria]
disciplina: Linguagens de Programação
fontes: [lp-a04-programacao-estruturada-linguagem-c]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Escopo de Variáveis

## Definição

O **escopo** de uma variável define em que parte do código ela existe e pode ser acessada. Em C (e em muitas outras linguagens), variáveis declaradas **dentro de uma função** têm escopo local: são criadas quando a função começa a ser executada e destruídas quando ela termina.

> "Variáveis declaradas dentro de uma função são ativas apenas durante a execução da função, tendo sido criada no momento da execução da função, e tendo o espaço ocupado pela mesma na memória liberada assim que a função é encerrada." (LP A4)

## Consequência Prática

Como parâmetros de função em C são passados por **valor** (cópia), modificar os parâmetros internos de uma função **não altera** as variáveis originais externas:

```c
// a e b dentro da função são cópias; os originais não mudam
void trocaValores(int a, int b) {
    int aux = a;
    a = b;
    b = aux;
}
```

Para modificar variáveis externas, é necessário usar [Ponteiros](ponteiros.md) (passagem por referência).

## Relações

- [Ponteiros](ponteiros.md) — mecanismo para contornar limitações de escopo local
- [Linguagem C](linguagem-c.md) — linguagem onde o escopo local é regra padrão para variáveis de funções

## Fontes

- [LP A4 — Programação Estruturada: Linguagem C](../fontes/lp-a04-programacao-estruturada-linguagem-c.md)
