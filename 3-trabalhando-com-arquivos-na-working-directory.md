# 3. Trabalhando com arquivos na working directory

**1 Removendo arquivo com status "deleted" da arvore**
```bash
git rm nome-file.extensao
```

**2 Removendo arquivo(s) com status "deleted" da arvore**
```bash
git add --all
```

**3 Deletando todos os arquivos da arvore e do projeto**
```bash
git rm -rf . ( CUIDADO )
```

**4 Removendo pastas da arvore**
```bash
git rm -r nome-diretorio
```

**5 Removendo pastas da staged area e git directory**
```bash
git rm -rf nome-diretorio/ --cached
```
