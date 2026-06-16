---
titulo: Compilação e Interpretação
tipo: conceito
tags: [compilacao, interpretacao, bytecode, jvm, java, linguagens]
disciplina: Linguagens de Programação
fontes: [lp-a03-programacao-estruturada-conceitos]
criado: 2026-05-11
atualizado: 2026-05-11
---

# Compilação e Interpretação

## Definição

São os dois processos fundamentais pelos quais código-fonte escrito por um programador é avaliado e executado.

---

## Compilação

Processo em etapas que transforma código-fonte em software executável independente:

1. **Análise léxica** — caracteres agrupados em lexemas (tokens: palavras reservadas, identificadores, valores)
2. **Análise sintática** — tokens organizados em árvore léxica; verifica se comandos estão bem formados (Sebesta, 2011)
3. **Análise semântica** — avalia a estrutura completa; instruções estão nos lugares corretos?
4. **Arquivo objeto** — código intermediário sem comentários, estrutura já validada
5. **Linkador** — agrega bibliotecas externas ao objeto → gera o **executável final**

**Limitação de portabilidade**: executáveis nativos são específicos para cada plataforma (SO + hardware). O mesmo código-fonte deve ser recompilado em cada plataforma.

---

## Interpretação

Código-fonte analisado e **executado diretamente** por um interpretador, sem gerar executável independente.

| Variante | Comportamento |
|----------|---------------|
| Permissiva (navegadores web) | Erros ignoráveis são descartados; execução continua com os elementos válidos |
| Rigorosa | Análise prévia completa (sintaxe + semântica) antes de executar; pode gerar arquivos temporários |

---

## Bytecode / Compilação Parcial

Caminho intermediário: compila o código-fonte até um **arquivo bytecode** (objeto portável), que é depois **interpretado por uma máquina virtual**.

- **Exemplo canônico**: Java — código `.java` → `.class` (bytecode) → interpretado pela JVM
- **Alta portabilidade**: mesmo bytecode roda em qualquer plataforma com a máquina virtual instalada
- Contraste com compilação clássica: não é um executável nativo, mas também não é código-fonte bruto

---

## Resumo Comparativo

| Processo | Gera executável? | Portabilidade | Exemplo |
|----------|-----------------|---------------|---------|
| Compilação clássica | Sim (nativo) | Baixa | C, C++ |
| Interpretação | Não | Alta (depende do interpretador) | JavaScript, PHP |
| Bytecode | Parcial (portável) | Alta (JVM presente) | Java |

## Relações

- [Sintaxe e Semântica](sintaxe-e-semantica.md) — etapas de análise presentes em compiladores e interpretadores rigorosos
- [Linguagem C](linguagem-c.md) — linguagem compilada clássica
- [Critérios de Avaliação de Linguagens](criterios-avaliacao-linguagens.md) — portabilidade é um dos critérios de Sebesta

## Fontes

- [LP A3 — Programação Estruturada: Conceitos](../fontes/lp-a03-programacao-estruturada-conceitos.md)
- [ALP A03 — Análise de Problemas e Elaboração de Soluções Computacionais](../fontes/alp-a03-analise-problemas-algoritmos.md)
- [Sebesta (2011)](../autores/sebesta.md)
