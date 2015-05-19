# 4. Trabalhando com commits

**4.1** Commitando arquivos 

git commit -m "Inseir um Comentário Significativo"

**4.2** Editando o último commit

git commit --amend -m "mensagem-do-commit"

**4.3** revertendo ação de um commit específico

git revert commit-hash

**4.4** Visualizando relatório de commits 

git log // Todos os commits

git log --pretty==oneline // Visualizando somente o código e mensagem de cada commit

git log -p // Junção dos Commits realizados + Diff

git log -p // Quantidade específica de Commits realizados + Diff

gitk // Visualize os Commits numa interface gráfica