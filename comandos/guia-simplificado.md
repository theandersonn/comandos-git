# Guia simplificado

###1 Configurações iniciais do Git

**Baixando e instalando o Git**
```bash
https://git-scm.com/downloads
```

**Configura nome de usuário**
```bash
git config --global user.name nome-sobrenome
```

**Configura email de usuário**
```bash
git config --global user.email email@email.com.br
```

###2 Inicializando um repositório

**Inicializa o versionamento no respectivo diretório**
```bash
git init
```

###3 Comandos básicos para sobreviver

**Verifica o status do repositório**
```bash
git status
```

**Adiciona todos os arquivos para serem commitados**
```bash
git add .
```

**Commitando arquivos**
```bash
git commit -m "inserir um comentário significativo"
```

**Visualizando relatório de commits**
```bash
git log // todos os commits
git log --oneline // exibe log com hash e título do commit
```

**Enviando as modificações para o repositório remoto**
```bash
git push origin <branch>
```

**Puxando alterações do repositório remoto**
```bash
git pull origin <branch>
```

###4 Trabalhando com branchs

**Criando e locomovendo-se para uma nova branch**
```bash
git checkout -b nome-branch 
```

**Aplicando merge em branchs**
```bash
git merge nome-branch // precisa estar na branch de destino
```

**Visualizando todas as branches existentes no repositório**
```bash
git branch
```

**Deletando uma branch local**
```bash
git branch -D nome-branch
```

**Deletando uma branch remoto**
```bash
git push origin :nome-branch
```

