# 3. Trabalhando com arquivos na working directory

**1 Removendo arquivos "deleted" da arvore**
```bash
git rm nome-file.extensao
```
**2 Deletando todos os arquivos da arvore e do projeto**
```bash
git rm -rf . ( CUIDADO )
```
**3 Removendo pastas da arvore**
```bash
git rm -r nome-diretorio
```

**4 Removendo pastas da staged area e git directory**
```bash
git rm -rf nome-diretorio/ --cached
```
