---
title: ip
draft: false
tags:
  - 
---
# Comando `ip`

O comando **`ip`** é uma ferramenta moderna para manipulação de interfaces de rede, substituindo o `ifconfig`.

## Sintaxe básica
    ip [opções] [objeto] [comando]

## Exemplos
- **Exibir informações de todas as interfaces**:
      ip addr show

- **Ativar uma interface**:
      ip link set eth0 up

- **Adicionar um endereço IP**:
      ip addr add 192.168.1.100/24 dev eth0

## Links Relacionados
- [[ifconfig]]: Comando antigo para manipulação de interfaces de rede.
- [[tcpdump]]: Comando para capturar pacotes de rede.