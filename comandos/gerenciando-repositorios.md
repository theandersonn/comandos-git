# Gerenciando Repositórios

**1 Pesquisa de texto em todos os diretórios**
```bash
git grep termo-da-busca
```

**2 Visualizando relatório de commits**
```bash
gitk // Visualize os Commits numa interface gráfica

git log // Todos os commits

git log -p // Commits realizados + Diff

git log -p -3 // Commits realizados + Diff com limitação de exibição

git log --stat // Resultado com estatistica

git log --name-status // Visualiza status de todos os arquivos que foram modificados

git log --oneline // Exibe log com hash e título do commit

git log --pretty=oneline // Visualizando somente o código e mensagem de cada commit

git log --abbrev-commit // Abrevia hash-commit

git log --pretty=oneline --abbrev-commit // Resulta em linha única com hash-commit abreviada

git log --pretty=format:"%h - %an, %ar : %s" // Resultado personalizado com hash - autor - tempo - titulo-commit

```

**3 Visualizar número de commits por usuário**
```bash
git shortlog -s
```

**4 Visualizar alterações feitas depois do último commit que ainda não foram stageadas**
```bash
git diff
```

**5 Visualizar alterações feitas depois do último commit que já foram stageadas**
```bash
git diff --cached
```

**6 Identificando User que fez alterações em determinado arquivo**
```bash
git blame nome-arquivo
```
