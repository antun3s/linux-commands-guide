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
```bash
grep "palavra" arquivo.txt
```

- **Buscar recursivamente em diretórios**:
```bash
grep -r "palavra" /caminho/
```
- **Ignorar maiúsculas/minúsculas**:
```bash
grep -i "palavra" arquivo.txt
```
- **Inverter a busca (excluir linhas que contêm o padrão)**:
```bash
grep -v "palavra" arquivo.txt
```
- **Exibir apenas a parte correspondente ao padrão**:
```bash
grep -o "palavra" arquivo.txt
```
- **Contar o número de ocorrências**:
```bash
grep -c "palavra" arquivo.txt
```
- **Exibir o número da linha onde o padrão foi encontrado**:
```bash
grep -n "palavra" arquivo.txt
```
- **Buscar por padrões usando expressões regulares**:
```bash
grep "^inicio" arquivo.txt  # Linhas que começam com "inicio"
grep "fim$" arquivo.txt     # Linhas que terminam com "fim"
```
- **Buscar por múltiplos padrões**:
```bash
grep -e "padrao1" -e "padrao2" arquivo.txt
```
- **Exibir linhas antes e depois do padrão**:
```bash
grep -A 2 "palavra" arquivo.txt  # Exibe 2 linhas após o padrão
grep -B 2 "palavra" arquivo.txt  # Exibe 2 linhas antes do padrão
grep -C 2 "palavra" arquivo.txt  # Exibe 2 linhas antes e depois
```
## Opções comuns
- **`-i`**: Ignora maiúsculas/minúsculas.
- **`-v`**: Inverte a busca (exclui linhas que contêm o padrão).
- **`-o`**: Exibe apenas a parte correspondente ao padrão.
- **`-c`**: Conta o número de ocorrências.
- **`-n`**: Exibe o número da linha onde o padrão foi encontrado.
- **`-r`**: Busca recursivamente em diretórios.
- **`-e`**: Permite especificar múltiplos padrões.
- **`-A`**: Exibe linhas após o padrão.
- **`-B`**: Exibe linhas antes do padrão.
- **`-C`**: Exibe linhas antes e depois do padrão.

## Links Relacionados
- [[find]]: Busca arquivos por critérios.
- [[awk]]: Processa texto em arquivos.
- [[sed]]: Edita texto em arquivos.
