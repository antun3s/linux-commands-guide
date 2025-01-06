---
title: sed
draft: false
tags:
  - 
---
# Comando `sed`

O comando **`sed`** (Stream Editor) é usado para editar texto em arquivos de forma eficiente, principalmente em fluxos de texto ou arquivos grandes.

## Sintaxe básica
```bash
sed [opções] 'comando' [arquivo]
```
## Exemplos
- **Substituir texto**:
```bash
sed 's/antigo/novo/' arquivo.txt
```

- **Substituir globalmente (todas as ocorrências na linha)**:
```bash
sed 's/antigo/novo/g' arquivo.txt
```

- **Substituir apenas a N-ésima ocorrência em cada linha**:
```bash
sed 's/antigo/novo/2' arquivo.txt  # Substitui a segunda ocorrência
```

- **Substituir texto em uma linha específica**:
```bash
sed '5s/antigo/novo/' arquivo.txt  # Substitui apenas na linha 5
```

- **Excluir linhas**:
```bash
sed '5d' arquivo.txt  # Exclui a linha 5
sed '1,3d' arquivo.txt  # Exclui as linhas de 1 a 3
sed '/padrao/d' arquivo.txt  # Exclui linhas que contêm "padrao"
```

- **Exibir apenas linhas específicas**:
```bash
sed -n '5p' arquivo.txt  # Exibe apenas a linha 5
sed -n '1,3p' arquivo.txt  # Exibe as linhas de 1 a 3
sed -n '/padrao/p' arquivo.txt  # Exibe linhas que contêm "padrao"
```

- **Inserir texto antes ou depois de uma linha**:
```bash
sed '5i\texto' arquivo.txt  # Insere "texto" antes da linha 5
sed '5a\texto' arquivo.txt  # Insere "texto" depois da linha 5
```

- **Substituir texto apenas em linhas que correspondem a um padrão**:
```bash
sed '/padrao/s/antigo/novo/' arquivo.txt
```

- **Editar o arquivo diretamente (salvar alterações)**:
```bash
sed -i 's/antigo/novo/' arquivo.txt  # Edita o arquivo original
sed -i.bak 's/antigo/novo/' arquivo.txt  # Cria um backup antes de editar
```

- **Executar múltiplos comandos**:
```bash
sed -e 's/antigo/novo/' -e '5d' arquivo.txt
```

- **Substituir texto usando expressões regulares**:
```bash
sed 's/^inicio/novo/' arquivo.txt  # Substitui no início da linha
sed 's/fim$/novo/' arquivo.txt  # Substitui no final da linha
sed 's/[0-9]*/NÚMERO/' arquivo.txt  # Substitui números por "NÚMERO"
```

## Opções comuns
- **`-n`**: Suprime a saída automática (usado com `p` para exibir linhas específicas).
- **`-i`**: Edita o arquivo diretamente (salva as alterações).
- **`-e`**: Permite executar múltiplos comandos.
- **`-r`**: Usa expressões regulares estendidas (equivalente a `-E`).

## Links Relacionados
- [[awk]]: Processa texto em arquivos.
- [[grep]]: Filtra conteúdo de arquivos.
- [[find]]: Busca arquivos por critérios.
