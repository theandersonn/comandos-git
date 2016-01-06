# Configurações

**Obs1:** (Exemplo Windows) Acesse o menu iniciar, localize o ícone do Git Bash, clique com o direito do mouse e em propriedades altere para o local onde normalmente ficam os seus projetos. Exemplo: D:\xampp\htdocs

**Obs2:** No Git Bash a maioria dos comandos são inicializados com $, no entanto são inseridos automaticamente pela ferramenta. Por este motivo ocultei nos exemplos abaixo.


**1 Locomovendo-se pelas pastas do projeto**
```bash
cd nome-da-pasta

cd .. // Retorna 1 nível

cd - // Retorna para a pasta que estávamos anteriormente
```

**2 Retorna o caminho da pasta atual**
```bash
pwd
```

**3 Abre o Windows Explorer**
```bash
explorer
```

**4 Abre o Explorer do Windows na pasta que estamos atualmente**
```bash
explorer .
```

**5 Configura nome de usuário**
```bash
git config --global user.name nome-de-usuario
```

**6 Configura email de usuário**
```bash
git config --global user.email email@email.com.br
```

**7 Configura editor padrão**
```bash
git config --global core.editor nome-editor
```

**8 Configura a mergetool (meld)**
```bash
git config --global merge.tool meld
```

**9 Edita configurações globais**
```bash
git config --global -e

// Exemplo editor = atom --wait
```

**10 Armazena senha (https)**
```bash
git config --global credential.helper cache
```

**11 Remove senha armazenada (https)**
```bash
git config --global --unset credential.helper
```

**12 armazena senha temporariamente (https)**
```bash
git config --global credential.helper 'cache --timeout=3600' // (3600 segundos = 1 hora)
```

**13 Remove configuração setada**
```bash
git config --global --unset propriedade
git config --global --unset core.editor // exemplo
git config --global --unset user.email // exemplo
```

**14 Visualiza as configurões de usuário**
```bash
git config -l
```

**15 Visualiza as configurões de usuário**
```bash
git config --list
```

**16 Verifica versão do git bash**
```bash
git --version
```
