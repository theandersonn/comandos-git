# 7. Trabalhando com Git e GitHub

**7.1 Gerando uma chave SSH de autenticação no Git bash**
```bash
// O git irá lhe perguntar: "nome de arquivo" e "senha", aplique 2 enters e ignore se for conveniente
ssh-keygen

// Normalmente o Git gera essa chave numa pasta dentre de Meus Documentos

Abra o arquivo ".ssh > id_rsa" e copie a chave
```
**7.2 Configurando a chave SSH no GitHub**
```bash
// Insira um nome para identificar a sua máquina no Github

// No Github vá em "Settings > SSH Keys" (Title + Key)
```
**7.3 Crie um repositorio no GitHub**
```bash
Acesse "Repositories" > New
```
**7.4 Clonando o repositório para a sua máquina**
```bash
No Github copie a URL SSH

No gitBash (git clone + insert nomeOpcional)
```
**7.5 Enviando as modificações para o GitHub**
```bash
git push origin master
```
**7.6 Deletando branch remota**
```bash
git push origem :nome-da-branch
```
**7.7 Baixando as modificações do GitHub para a sua máquina** (Se o repositório for de sua autoria)
```bash
git pull origin master
```
**7.8 Mantendo o Repositório Forkado atualizado com o original** (Para repositórios forkados)
```bash
// Nesse momento o nosso repositório chama-se "origin";
// Vamos criar um novo chamado "upstream" que apontará para o original.

git remote add upstream insira-url-ssh-do-repositorio-original
```
**7.9 Sincronizando os dois repositórios** (upstream e original)
```bash
git fetch upstream
```
**7.10 Aplicando merge nas atualizações do fork para a branch master do nosso repositório**
```bash
git merge upstream/master
```
