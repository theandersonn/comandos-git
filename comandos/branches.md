# Trabalhando com branches

**Criar uma nova branch**
```bash
git branch nome-branch

# Acessando a nova branch
git checkout nome-branch 

# Criando e acessando uma nova branch
git checkout -b nome-branch 

# Criando uma nova branch vazia
git checkout --orphan nome-branch 
```

**Baixar todas as branchs que estão online**
```bash
git fetch --all ou git remote update
```

**Criar uma branch local baseada na remota**
```bash
git fetch origin 

git checkout origin/feature-x -b feature-x
```

**Renomeiar branch local**
```bash
# Renomeia a brach localmente
git branch -m old-branch new-branch 

# Deleta a branch velha
git push --set-upstream origin new-branch

# Empurra a nova branch, define a branch local no track remoto
git push origin :old-branch  
```

**Retorna num ponto específico e cria uma nova branch**
```bash
git checkout hash-commit -b nome-nova-branch
```

**Renomeando branches**
```bash
git branch -m nome-branch
```

**Aplicando merge em branches**
```bash
# Precisa estar na branch de destino
git merge nome-branch 
```

**Visualizando todas as branches existentes no repositório**
```bash
# A branch corrente será marcada por um asterisco
git branch 
```

**Visualizando todas as branches locais e remotas**
```bash
git branch -a
```

**Deletando uma branch**
```bash
git branch -D nome-branch
```

**Deletando branch remota**
```bash
git push origin :nome-branch
```
