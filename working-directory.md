# Trabalhando com arquivos na working directory

**1 Adiciona aquivos para serem commitados**
```bash
1. maneira: git add nome-do-aquivo.extensao

2. maneira: git add *.extensao

3. maneira: git add . //add todos

4. maneira: git add --all //add todos incluindo deletados
```

**2 Removendo arquivo da Working Directory**
```bash
git checkout nome-arquivo.extensao
```

**3 Removendo arquivo com status "deleted" da arvore**
```bash
git rm nome-file.extensao
```

**4 Removendo arquivo(s) com status "deleted" da arvore**
```bash
git add --all
```

**5 Deletando todos os arquivos da arvore e do projeto**
```bash
git rm -rf . ( CUIDADO )
```

**6 Removendo pastas da arvore**
```bash
git rm -r nome-diretorio
```

**7 Removendo pastas da staged area e git directory**
```bash
git rm -rf nome-diretorio/ --cached
```
