# 4. Trabalhando com arquivos na stage area

**4.1 Visualizando a última alteração feita**
```bash
git diff // no diretório de trabalho (compara Work Directory com Staging Area)

git diff --staged // na staged area (compara Staging Area com .Git Directory)

git diff nome-arquivo.extensao // Visualiza alterações específicas de um commit
```
**4.2 Revertendo alterações feitas em arquivos** (Arquivos que estão na área de trabalho)
```bash
git checkout -- nome-do-arquivo.extensao
```
**4.3 Adicionando aquivos na stage area**
```bash
1. maneira: git add nome-do-aquivo.extensao

2. maneira: git add *.extensao

3. maneira: git add . //add todos
```
**4.4 Removendo aquivos da stage area**
```bash
git reset HEAD nome-do-aquivo.extensao
```
**4.5 Limpando a stage area (Removendo arquivos que foram deletados)**
```bash
git rm nome-do-arquivo.extensao
```
