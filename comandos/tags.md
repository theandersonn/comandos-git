# Trabalhando com Tags

**1 Crianddo Lightweight Tag**

```bash
# É recomendado utiliza-la somente localmente.
git tag "1.0.0"
```

**2 Crianddo Annotated Tag**

```bash
# É recomendado utiliza-la para servidos, ou seja tags de release.
git tag -a "1.0.0" -m "1.0.0"
```

**3 Listando as Tags criadas**

```bash
git tag
```

**4 Enviando as Tags criadas para o servidor**

```bash
# enviará as tags do tipo Annotated 
git push origin master --follow-tags
```