# 5. Trabalhando com commits

**5.1 Commitando arquivos**
```bash
git commit -m "Inseir um Comentário Significativo"
```

**5.2 Commitando arquivos já inseridos na Staging Area**
```bash
git commit -a -m "Inseir um Comentário Significativo"
```

**5.3 Editando o último commit**
```bash
git commit --amend -m "mensagem-do-commit"
```

**5.4 Revertendo ação de um commit específico**
```bash
git revert commit-hash
```

**5.5 Abortando o merge**
```bash
git merge --abort
```

**5.6 Acionando a merge tool**
```bash
git merge tool
```

**5.7 Excluindo um commit local**
```bash
git reset --hard numero-hash-commit
```

**5.8 Visualizando relatório de commits**
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

**5.9 Visualizar número de commits por usuário**
```bash
git shortlog -s
```

**5.10 Visualizar alterações feitas depois do último commit que ainda não foram stageadas**
```bash
git diff
```

**5.11 Visualiza alterações específicas**
```bash
git diff nome-arquivo.extensao
```

**5.12 Visualiza alterações entre commits**
```bash
git diff hash-commit1 hash-commit2
```

**5.13 Identificando User que fez alterações em determinado arquivo**
```bash
git blame 'nome-arquivo'
```

**5.14 Visualizar alterações feitas depois do último commit que já foram stageadas**
```bash
git diff --cached
```

**5.15 Transferindo alterações que ainda não estão commitadas para o stash**
```bash
git stash
```

**5.16 Visualizando itens que estão no stash**
```bash
git stash list
```

**5.17 Utilizando o último item adicionado no stash**
```bash
git stash apply
```

**5.18 Limpando o stash**
```bash
git stash clear
```
