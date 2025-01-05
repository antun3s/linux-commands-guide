---
title: awk
draft: false
tags:
  - 
---
# Comando `awk`

O comando **`awk`** é uma linguagem de programação para processamento de texto.

## Sintaxe básica
    awk [opções] 'script' [arquivo]

## Exemplos
- **Exibir a primeira coluna de um arquivo**:
      awk '{print $1}' arquivo.txt

- **Filtrar linhas com uma condição**:
      awk '$3 > 100 {print $0}' arquivo.txt

- **Usar delimitador personalizado**:
      awk -F',' '{print $2}' arquivo.csv

## Links Relacionados
- [[grep]]: Filtra conteúdo de arquivos.
- [[sed]]: Edita texto em arquivos.