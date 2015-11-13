# 5. Trabalhando com commits

**1 Commitando arquivos**
```bash
git commit -m "Inseir um Comentário Significativo"
```

**2 Commitando arquivos já inseridos na Staging Area**
```bash
git commit -a -m "Inseir um Comentário Significativo"
git commit -am "Inseir um Comentário Significativo"
```

**3 Editando a mensagem do último commit**
```bash
git commit --amend -m "mensagem-do-commit"
```

**4 Fechar issues através de commits**
```bash
git commit -m "Mensagem commit - fix ou resolve IDissue"
```

**5 Revertendo ação de um commit específico**
```bash
git revert commit-hash
```

**6 Abortando o processo de reverter commit**
```bash
git revert --abort
```

**7 Abortando o merge**
```bash
git merge --abort
```

**8 Acionando a merge tool**
```bash
git merge tool
```

**9 Excluindo um commit local**
```bash
git reset --hard numero-hash-commit
```

**10 Visualizando relatório de commits**
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

**11 Visualizar número de commits por usuário**
```bash
git shortlog -s
```

**12 Visualizar alterações feitas depois do último commit que ainda não foram stageadas**
```bash
git diff
```

**13 Visualiza alterações específicas**
```bash
git diff nome-arquivo.extensao
```

**14 Visualiza alterações entre commits**
```bash
git diff hash-commit1 hash-commit2
```

**15 Visualiza arquivos em conflito**
```bash
git diff --name-only --diff-filter=U
```

**16 Identificando User que fez alterações em determinado arquivo**
```bash
git blame nome-arquivo
```

**17 Visualizar alterações feitas depois do último commit que já foram stageadas**
```bash
git diff --cached
```

**18 Transferindo alterações que ainda não estão commitadas para o stash**
```bash
git stash
```

**19 Visualizando itens que estão no stash**
```bash
git stash list
```

**20 Utilizando o último item adicionado no stash**
```bash
git stash apply
```

**21 Remove Stash**
```bash
git stash drop stash@{0}
```

**22 Aplica e remove o último Stash**
```bash
git stash pop
```

**23 Limpando o stash**
```bash
git stash clear
```
