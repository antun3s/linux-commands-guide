---
title: grep
draft: false
tags:
  - 
---
# Comando `grep`

O comando **`grep`** (Global Regular Expression Print) é usado para filtrar conteúdo de arquivos com base em padrões.

## Sintaxe básica
    grep [opções] [padrão] [arquivo]

## Exemplos
- **Buscar uma palavra em um arquivo**:
      grep "palavra" arquivo.txt

- **Buscar recursivamente**:
      grep -r "palavra" /caminho/

- **Ignorar maiúsculas/minúsculas**:
      grep -i "palavra" arquivo.txt

## Links Relacionados
- [[find]]: Busca arquivos por critérios.
- [[awk]]: Processa texto em arquivos.