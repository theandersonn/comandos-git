# Trabalhando com commits

**1 Commitando arquivos**

*Depois de adicionar os arquivos com git add -A, por exemplo.*

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

O ID da Issue você consegue na URL da mesma. Ex.: `issues/8` - 8.

Outras palavras chave que podemos usar para fechamento de Issues: `fix, fixes, fixed, close, closes, closed, resolve, resolves, resolved`

**5 Revertendo ação de um commit específico**
```bash
git revert commit-hash
```

Para encontrar o hash, você precisa rodar no terminal: `git log`.

O hash é aquele número que aparece em `comit: xxxxxxx.`

**6 Abortando o processo de reverter commit**
```bash
git revert --abort
```

**7 Abortando o merge**
```bash
git merge --abort
```

**8 Acionando a [mergetool](https://git-scm.com/docs/git-mergetool)**
```bash
git mergetool
```

**9 Excluindo um commit local**
```bash
git reset --hard hash-commit
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

**16 Transferindo alterações que ainda não estão commitadas para o stash**
```bash
git stash
```

**17 Visualizando itens que estão no stash**
```bash
git stash list
```

**18 Utilizando o último item adicionado no stash**
```bash
git stash apply
```

**19 Remove Stash**
```bash
git stash drop stash@{0}
```

**20 Aplica e remove o último Stash**
```bash
git stash pop
```

**21 Limpando o stash**
```bash
git stash clear
```
