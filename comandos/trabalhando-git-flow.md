# Trabalhando com Git Flow

### Git Flow

> Aqui é apenas um resumo  
> Nem todos os comandos disponíveis estão cobertos aqui, apenas os mais importantes deles

**O que é?**

> O git-flow é um conjunto de extensões para o git que provê operações de alto-nível para repositórios usando o modelo de branches do Vincent Driessen  
> Você pode continuar a usar o git e todos os comandos dele normalmente como você já conhece, o git flow é apenas uma coleção de ferramentas

*Em poucas palavras*
> Uma forma de organização usando branches

**Funcionamento**

*Git Flow é divido em 3 tageamentos:*
- Funcionalidades / Feature;
- Versão / Release;
- Hotfix

### Instalação


**Ubuntu/Debian-based**
```bash
sudo apt-get install git-flow
```


**Mac OS X**
```bash
brew install git-flow-avh
```


**Windows**
*(Cygwin)*
```bash
wget -q -O - --no-check-certificate https://raw.github.com/petervanderdoes/gitflow-avh/develop/contrib/gitflow-installer.sh install stable | bash
```
*Ou*
```bash
https://git-for-windows.github.io/
```
> A partir do Git Windows 2.6.4, GitFlow (AVH) está incluído.


**Manual**
```bash
wget --no-check-certificate -q  https://raw.github.com/petervanderdoes/gitflow-avh/develop/contrib/gitflow-installer.sh && bash gitflow-installer.sh install stable; rm gitflow-installer.sh
```


### Começando com Git Flow


**Inicialização**
*Para começar a usar Git Flow em seu projeto, você precisa iniciá-lo*
```bash
git flow init
```


##Funcionalidade / Features
> O desenvolvimento de uma nova funcionalidade começa a partir do ponto atual de seu branch DEVELOP

**Começar uma nova funcionalidade**
```bash
git flow feature start MINHA_FUNCIONALIDADE
```
> Criar um branch (baseado no develop) e automaticamente irá dar uma checkout nesse branch

**Finalizando uma funcionalidade**
```bash
git flow feature finish MINHA_FUNCIONALIDADE
```
> Esse comando irá executar as seguintes ações:  
> Merge com a branch develop;  
> Deleta a branch funcionalidade;  
> Checkout na branch develop;  
> Para finalizar uma funcionalidade, você deve executar esse comando dentro do branch funcionalidade que deseja finalizar

**Publicando uma funcionalidade**
```bash
git flow feature publish MINHA_FUNCIONALIDADE
```

**Obter uma funcionalidade**
```bash
git flow feature pull MINHA_FUNCIONALIDADE
```
> Simplesmente um pull de uma branch

## Versões / Release
> Auxilia a preparação de uma nova versão de produção

**Começar uma nova versão**
```bash
git flow release start MINHA_VERSAO
```
> Cria um branch baseado no develop

**Publicando uma versão**
```bash
git flow release publish MINHA_VERSAO
```
> É sensato publicar o branch da versão depois de criá-lo, para permitir commits por outros desenvolvedores

**Finalizar uma versão**
```bash
git flow release finish MINHA_VERSAO
```
> Na finalização de uma versão, ele executa várias ações:  
> Faz merge do branch MINHA_VERSAO no MASTER;  
> Faz merge do branch MINHA_VERSAO e um checkout no DEVELOP;  
> Etiqueta a versão com seu nome;  
> Remove o branch MINHA_VERSAO;

## Hotfix
> Os hotfixes surgem da necessidade de agir imediatamente sobre uma situação indesejada na versão de produção ativa

**Criando um hotfix**
```bash
git flow hotfix start MEU_HOTFIX
```
> Cria um branch baseado no MASTER  
> O argumento MEU_HOTFIX nesse caso marca a versão defeituosa na produção

**Finalizar um hotfix**
```bash
git flow hotfix finish MEU_HOTFIX
```
> Ele irá fazer um merge no MASTER e no DEVELOP  
> O merge no MASTER será etiquetado

### Resumo dos Comandos
![Git Flow Comandos] (../images/git-flow-comandos.png)

### Fonte
Git-Flow: https://github.com/nvie/gitflow  
Documentação: http://danielkummer.github.io/git-flow-cheatsheet/
