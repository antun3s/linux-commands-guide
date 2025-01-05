---
title: curl
draft: false
tags:
  - 
---
# Comando `curl`

O comando **`curl`** é usado para transferir dados de/para servidores usando vários protocolos.

## Sintaxe básica
    curl [opções] [URL]

## Exemplos
- **Baixar um arquivo**:
      curl -O https://exemplo.com/arquivo.txt

- **Enviar dados via POST**:
      curl -X POST -d "dados=valor" https://exemplo.com

- **Verificar cabeçalhos**:
      curl -I https://exemplo.com

## Links Relacionados
- [[wget]]: Baixa arquivos da web.
- [[ssh]]: Conecta-se a servidores remotos.