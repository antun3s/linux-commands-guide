---
title: rsync
draft: false
tags:
  - 
---
# Comando `rsync`

O comando **`rsync`** (Remote Sync) é usado para sincronizar arquivos e diretórios entre sistemas locais ou remotos de forma eficiente.

## Sintaxe básica
    rsync [opções] [origem] [destino]

## Exemplos
- **Sincronizar arquivos localmente**:
      rsync -av /caminho/origem/ /caminho/destino/

- **Sincronizar com um servidor remoto**:
      rsync -av /caminho/local/ usuario@192.168.1.1:/caminho/remoto/

- **Sincronizar de um servidor remoto para local**:
      rsync -av usuario@192.168.1.1:/caminho/remoto/ /caminho/local/

- **Excluir arquivos específicos**:
      rsync -av --exclude='*.tmp' /caminho/origem/ /caminho/destino/

- **Sincronizar e excluir arquivos no destino que não existem na origem**:
      rsync -av --delete /caminho/origem/ /caminho/destino/

## Opções comuns
- **`-a`**: Modo de arquivamento (preserva permissões, timestamps, etc.).
- **`-v`**: Modo verboso (exibe detalhes do processo).
- **`-z`**: Comprime dados durante a transferência.
- **`-r`**: Sincroniza diretórios recursivamente.
- **`--delete`**: Exclui arquivos no destino que não existem na origem.
- **`--exclude`**: Exclui arquivos ou diretórios específicos.

## Links Relacionados
- [[scp]]: Copia arquivos entre sistemas via SSH.
- [[tar]]: Compacta e descompacta arquivos.
- [[ssh]]: Conecta-se a servidores remotos.