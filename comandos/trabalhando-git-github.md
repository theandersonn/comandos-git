# Trabalhando com Git e GitHub

**1 Gerando uma chave SSH de autenticação no Git bash**
```bash
// aplique 2 enters para confirmar "nome de arquivo" e "senha", 
ssh-keygen

// Localize a chave em "Meus Documentos"

Abra o arquivo ".ssh > id_rsa.pub" e copie a chave
```

**2 Verificar se existe chave SSH configurada**
```bash
ls -al ~/.ssh
```

**3 Configurando a chave SSH no GitHub**
```bash
// Insira um nome para identificar a sua máquina no Github

// No Github vá em "Settings > SSH Keys" (Title + Key)
```

**4 Verificar qual chave SSH está setada**
```bash
ssh -T
```

**5 Crie um repositorio no GitHub**
```bash
Acesse "Repositories" > New
```

**6 Clonando o repositório para a sua máquina**
```bash
No Github copie a URL SSH

No gitBash (git clone + url-repositorio)
```

**7 Inserir caminho do repositorio remoto**
```bash
git remote add origin url-repositorio // origin é o nome do repositório remoto
```

**8 Remover caminho do repositorio remoto**
```bash
git remote rm origin // origin é o nome do repositório remoto
```

**9 Verificar caminho do repositorio remoto que está setado**
```bash
git remote -v
```

**10 Altera a url do repositório remoto (Máquina local > Github)**
```bash
git remote set-url origin url-repositorio
```

**11 Enviando as modificações para o GitHub**
```bash
git push origin master
```

**12 Deletando branch remota**
```bash
git push origin nome-branch --delete
git push origin :nome-da-branch
```

**13 Baixando as modificações do GitHub para a sua máquina** (Se o repositório for de sua autoria)
```bash
git pull origin master
```

**14 Forçando git pull** (Os arquivos que estão locais serão subscritos)
```bash
git fetch --all
git reset --hard origin/master
git pull origin master
```

**15 Mantendo o Repositório Forkado atualizado com o original**
```bash
// Nesse momento o nosso repositório chama-se origin;
// Vamos criar um novo chamado "upstream" que apontará para o original.

git remote add upstream insira-url-ssh-do-repositorio-original
```

**16 Sincronizando os dois repositórios** (upstream e original)
```bash
git fetch upstream
```

**17 Aplicando merge nas atualizações do fork para a branch master do nosso repositório**
```bash
git merge upstream/master
```

**18 Fechar issues através de commits**
```bash
git commit -m "Mensagem commit - fix issue #1"
```
