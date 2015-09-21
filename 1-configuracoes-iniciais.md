# 1. Configurações iniciais

**Obs1:** (Exemplo Windows) Acesse o menu iniciar, localize o ícone do Git Bash, clique com o direito do mouse e em propriedades altere para o local onde normalmente ficam os seus projetos. Exemplo: D:\xampp\htdocs

**Obs2:** No Git Bash a maioria dos comandos são inicializados com $, no entanto são inseridos automaticamente pela ferramenta. Por este motivo ocultei nos exemplos abaixo.

**Obs3:** Não seja tímido(a) peça um help pro Git
git help insira-verb


**1.1 Locomovendo-se pelas pastas do projeto**
```bash
cd nome-da-pasta

cd .. // Retorna 1 nível
```

**1.2 Retorna o caminho da pasta atual**
```bash
pwd
```

**1.3 Configura nome de usuário**
```bash
git config --global user.name nome-sobrenome
```

**1.4 Configura email de usuário**
```bash
git config --global user.email email@email.com.br
```

**1.5 Configura editor padrão**
```bash
git config --global core.editor nome-editor
```

**1.6 Edita configurações globais**
```bash
git config --global -e

// Exemplo editor = atom --wait
```

**1.7 Visualiza as configurões de usuário**
```bash
git config -l
```

**1.8 Visualiza as configurões de usuário**
```bash
git config --list
```

**1.9 Verifica versão do git bash**
```bash
git --version
```
