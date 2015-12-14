# Trabalhando com arquivos na stage area

**1 Visualizando a última alteração feita**
```bash
git diff // no diretório de trabalho (compara Work Directory com Staging Area)

git diff --staged // na staged area (compara Staging Area com .Git Directory)

git diff nome-arquivo.extensao // Visualiza alterações específicas de um commit

git diff -w // Visualiza alterações ignorando espaços
```

**2 Revertendo alterações feitas em arquivos** (Arquivos que estão na área de trabalho)
```bash
git checkout -- nome-do-arquivo.extensao
```

**3 Removendo aquivos da stage area**
```bash
git reset HEAD nome-do-aquivo.extensao
```
