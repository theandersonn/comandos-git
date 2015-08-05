# 5. Trabalhando com commits

**5.1 Commitando arquivos**

git commit -m "Inseir um Comentário Significativo"

**5.2 Editando o último commit**

git commit --amend -m "mensagem-do-commit"

**5.3 revertendo ação de um commit específico**

git revert commit-hash

**5.4 Visualizando relatório de commits**

git log // Todos os commits

git log --pretty==oneline // Visualizando somente o código e mensagem de cada commit

git log -p // Junção dos Commits realizados + Diff

git log -p // Quantidade específica de Commits realizados + Diff

gitk // Visualize os Commits numa interface gráfica

**5.5 Visualizar alterações feitas depois do último commit que ainda não foram stageadas**

git diff
