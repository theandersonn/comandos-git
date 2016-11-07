# Trabalhando com branches

**1 Cria uma nova branch**
```bash
git branch nome-branch

# Acessando a nova branch
git checkout nome-branch 

# Criando e acessando uma nova branch
git checkout -b nome-branch 

# Criando uma nova branch vazia
git checkout --orphan nome-branch 
```

**2 Cria uma branch local baseada na remota**
```bash
git fetch origin 

git checkout origin/feature-x -b feature-x
```

**3 Renomeia branch local**
```bash
# Renomeia a brach localmente
git branch -m old-branch new-branch 

# Deleta a branch velha
git push --set-upstream origin new-branch

# Empurra a nova branch, define a branch local no track remoto
git push origin :old-branch  
```

**4 Retorna num ponto específico e cria uma nova branch**
```bash
git checkout hash-commit -b nome-nova-branch
```

# Para encontrar o hash, você precisa rodar no terminal: `git log`.
# O hash é aquele número que aparece em `comit: xxxxxxx.`

**5 Renomeando branches**
```bash
git branch -m nome-branch
```

**6 Aplicando merge em branches**
```bash
# Precisa estar na branch de destino
git merge nome-branch 
```

**7 Visualizando todas as branches existentes no repositório**
```bash
# A branch corrente será marcada por um asterisco
git branch 
```

**8 Visualizando todas as branches locais e remotas**
```bash
git branch -a
```

**9 Deletando uma branch**
```bash
git branch -D nome-branch
```

**10 Deletando branch remota**
```bash
git push origin :nome-branch
```
