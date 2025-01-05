---
title: sed
draft: false
tags:
  - 
---
# Comando `sed`

O comando **`sed`** (Stream Editor) é usado para editar texto em arquivos.

## Sintaxe básica
    sed [opções] 'comando' [arquivo]

## Exemplos
- **Substituir texto**:
      sed 's/antigo/novo/' arquivo.txt

- **Substituir globalmente**:
      sed 's/antigo/novo/g' arquivo.txt

- **Excluir linhas**:
      sed '5d' arquivo.txt

## Links Relacionados
- [[awk]]: Processa texto em arquivos.
- [[grep]]: Filtra conteúdo de arquivos.