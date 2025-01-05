---
title: tcpdump
draft: false
tags:
  - 
---
# Comando `tcpdump`

O comando **`tcpdump`** é usado para capturar e analisar pacotes de rede.

## Sintaxe básica
    tcpdump [opções] [filtro]

## Exemplos
- **Capturar pacotes em uma interface específica**:
      tcpdump -i eth0

- **Capturar pacotes com um filtro de porta**:
      tcpdump port 80

- **Salvar a captura em um arquivo**:
      tcpdump -w captura.pcap

## Links Relacionados
- [[ifconfig]]: Comando para configurar e listar interfaces de rede.
- [[ip]]: Comando moderno para manipulação de interfaces de rede.