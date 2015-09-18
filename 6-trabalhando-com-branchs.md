# 6. Trabalhando com branchs

**6.1 Criando uma nova branch**
```bash
git branch nome-branch

git checkout nome-branch // Acessando a nova branch

git checkout -b nome-branch // Criando e acessando uma nova branch (Prefiro esse)

git checkout --orphan nome-branch // Criando uma nova branch vazia
```
**6.2 Renomeando branchs**
```bash
git branch -m nome-branch
```

**6.3 Aplicando merge em branchs**
```bash
git merge nome-branch // Precisa estar na branch de destino
```

**6.4 Visualizando todas as branchs existentes no repositório**
```bash
git branch // A branch corrente será marcada por um asterisco
```

**6.5 Visualizando todas as branches locais e remotas**
```bash
git branch -a
```

**6.6 Deletando uma branch**
```bash
git branch -D nome-branch
```

**6.7 Deletando branch remota**
```bash
git push origin :nome-branch
```
