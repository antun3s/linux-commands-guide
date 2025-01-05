---
title: scp
draft: false
tags:
  - 
---
# Comando `scp`

O comando **`scp`** (Secure Copy) é usado para copiar arquivos entre sistemas via SSH.

## Sintaxe básica
    scp [opções] [origem] [destino]

## Exemplos
- **Copiar um arquivo para um servidor remoto**:
      scp arquivo.txt usuario@192.168.1.1:/caminho/

- **Copiar um diretório**:
      scp -r diretorio/ usuario@192.168.1.1:/caminho/

## Links Relacionados
- [[ssh]]: Conecta-se a um servidor remoto.
- [[rsync]]: Sincroniza arquivos entre sistemas.