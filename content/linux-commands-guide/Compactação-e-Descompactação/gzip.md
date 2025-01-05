---
title: gzip
draft: false
tags:
  - 
---
# Comando `gzip`

O comando **`gzip`** é usado para compactar arquivos no formato GZIP.

## Sintaxe básica
    gzip [opções] [arquivo]

## Exemplos
- **Compactar um arquivo**:
      gzip arquivo.txt
  Isso cria um arquivo `arquivo.txt.gz` e remove o arquivo original.

- **Compactar mantendo o arquivo original**:
      gzip -c arquivo.txt > arquivo.txt.gz

- **Compactar recursivamente todos os arquivos em um diretório**:
      gzip -r diretorio/

- **Descompactar um arquivo**:
      gunzip arquivo.txt.gz
  Ou:
      gzip -d arquivo.txt.gz

## Opções comuns
- **`-c`**: Envia a saída para o terminal (não remove o arquivo original).
- **`-d`**: Descompacta o arquivo (equivalente a `gunzip`).
- **`-r`**: Compacta recursivamente arquivos em diretórios.
- **`-v`**: Exibe detalhes do processo de compactação.

## Links Relacionados
- [[tar]]: Compacta e descompacta arquivos em formato TAR.
- [[zip-unzip]]: Compacta arquivos em formato ZIP.