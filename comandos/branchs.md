# Trabalhando com branches

**1 Criando uma nova branch**
```bash
git branch nome-branch

git checkout nome-branch // Acessando a nova branch

git checkout -b nome-branch // Criando e acessando uma nova branch (Prefiro esse)

git checkout --orphan nome-branch // Criando uma nova branch vazia
```

**2 Retorna num ponto específico e cria uma nova branch**
```bash
git checkout hash-commit -b nome-nova-branch
```

Para encontrar o hash, você precisa rodar no terminal: `git log`.

O hash é aquele número que aparece em `comit: xxxxxxx.`

**3 Renomeando branches**
```bash
git branch -m nome-branch
```

**4 Aplicando merge em branches**
```bash
git merge nome-branch // Precisa estar na branch de destino
```

**5 Visualizando todas as branches existentes no repositório**
```bash
git branch // A branch corrente será marcada por um asterisco
```

**6 Visualizando todas as branches locais e remotas**
```bash
git branch -a
```

**7 Deletando uma branch**
```bash
git branch -D nome-branch
```

**8 Deletando branch remota**
```bash
git push origin :nome-branch
```
