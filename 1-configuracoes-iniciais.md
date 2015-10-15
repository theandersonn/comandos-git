# 1. Configurações iniciais

**Obs1:** (Exemplo Windows) Acesse o menu iniciar, localize o ícone do Git Bash, clique com o direito do mouse e em propriedades altere para o local onde normalmente ficam os seus projetos. Exemplo: D:\xampp\htdocs

**Obs2:** No Git Bash a maioria dos comandos são inicializados com $, no entanto são inseridos automaticamente pela ferramenta. Por este motivo ocultei nos exemplos abaixo.

**Obs3:** Não seja tímido(a) peça um help pro Git
git help insira-verb


**1 Locomovendo-se pelas pastas do projeto**
```bash
cd nome-da-pasta

cd .. // Retorna 1 nível
```

**2 Retorna o caminho da pasta atual**
```bash
pwd
```

**3 Configura nome de usuário**
```bash
git config --global user.name nome-sobrenome
```

**4 Configura email de usuário**
```bash
git config --global user.email email@email.com.br
```

**5 Configura editor padrão**
```bash
git config --global core.editor nome-editor
```

**6 Configura a merge tool (meld)**
```bash
git config --global merge.tool meld
```

**7 Edita configurações globais**
```bash
git config --global -e

// Exemplo editor = atom --wait
```

**8 Armazena senha (https)**
```bash
git config --global credential.helper cache
```

**8 Remove configuração setada**
```bash
git config --global --unset propriedade
git config --global --unset core.editor // exemplo
git config --global --unset user.email // exemplo
```

**9 Visualiza as configurões de usuário**
```bash
git config -l
```

**10 Visualiza as configurões de usuário**
```bash
git config --list
```

**11 Verifica versão do git bash**
```bash
git --version
```
