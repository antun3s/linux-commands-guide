---
title: find
draft: false
tags:
  - 
---
# Comando `find`

O comando **`find`** é usado para buscar arquivos e diretórios com base em critérios específicos.

## Sintaxe básica
    find [caminho] [expressão]

## Exemplos
- **Buscar arquivos por nome**:
      find /caminho/ -name "*.txt"

- **Buscar arquivos modificados nos últimos 7 dias**:
      find /caminho/ -mtime -7

- **Executar um comando nos arquivos encontrados**:
      find /caminho/ -name "*.log" -exec rm {} \;

## Links Relacionados
- [[grep]]: Filtra conteúdo de arquivos.
- [[awk]]: Processa texto em arquivos.