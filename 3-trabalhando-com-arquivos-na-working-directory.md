# 3. Trabalhando com arquivos na working directory

**1 Removendo arquivo da Working Directory**
```bash
git checkout nome-arquivo.extensao
```

**2 Removendo arquivo com status "deleted" da arvore**
```bash
git rm nome-file.extensao
```

**3 Removendo arquivo(s) com status "deleted" da arvore**
```bash
git add --all
```

**4 Deletando todos os arquivos da arvore e do projeto**
```bash
git rm -rf . ( CUIDADO )
```

**5 Removendo pastas da arvore**
```bash
git rm -r nome-diretorio
```

**6 Removendo pastas da staged area e git directory**
```bash
git rm -rf nome-diretorio/ --cached
```
