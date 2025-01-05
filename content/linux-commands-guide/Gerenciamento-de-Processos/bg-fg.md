---
title: bg-fg
draft: false
tags:
  - 
---
# Comandos `bg` e `fg`

Os comandos **`bg`** (Background) e **`fg`** (Foreground) são usados para gerenciar processos em segundo plano e primeiro plano.

## Sintaxe básica
    bg [ID do trabalho]
    fg [ID do trabalho]

## Exemplos
- **Colocar um processo em segundo plano**:
      bg %1

- **Trazer um processo para o primeiro plano**:
      fg %1

## Links Relacionados
- [[ps]]: Lista processos ativos.
- [[kill]]: Encerra processos.