# 5. Trabalhando com commits

**5.1 Commitando arquivos**
```bash
git commit -m "Inseir um Comentário Significativo"
```
**5.2 Editando o último commit**
```bash
git commit --amend -m "mensagem-do-commit"
```
**5.3 Revertendo ação de um commit específico**
```bash
git revert commit-hash
```
**5.4 Excluindo um commit local**
```bash
git reset --hard numero-hash-commit
```
**5.5 Visualizando relatório de commits**
```bash
git log // Todos os commits

git log --pretty==oneline // Visualizando somente o código e mensagem de cada commit

git log -p // Junção dos Commits realizados + Diff

git log -p // Quantidade específica de Commits realizados + Diff

git diff nome-arquivo.extensao // Visualiza alterações específicas

git diff hash-commit1 hash-commit2 // Vializa alterações entre commits

gitk // Visualize os Commits numa interface gráfica
```
**5.6 Visualizar número de commits por usuário**
```bash
git shortlog -s
```
**5.7 Visualizar alterações feitas depois do último commit que ainda não foram stageadas**
```bash
git diff
```
**5.8 Visualizar alterações feitas depois do último commit que já foram stageadas**
```bash
git diff --cached
```
**5.9 Transferindo alterações que ainda não estão commitadas para o stash**
```bash
git stash
```
**5.10 Visualizando itens que estão no stash**
```bash
git stash list
```
**5.11 Utilizando o último item adicionado no stash**
```bash
git stash apply
```
**5.12 Limpando o stash**
```bash
git stash clear
```
