# Blog d'Arturo Candela

Blog personal sobre tecnologia i desenvolupament de software, escrit en català/valencià.

🌐 **Visita el blog**: [arturocandela.github.io/blog](https://arturocandela.github.io/blog/)

## Sobre aquest projecte

Aquest és el meu espai personal per compartir:

- Notes de projectes personals
- Aprenentatges tècnics
- Entrades curtes amb proves i experiments
- Reflexions sobre desenvolupament de software

## Tecnologia

- **Framework**: [MkDocs](https://www.mkdocs.org/)
- **Tema**: [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- **Allotjament**: GitHub Pages
- **Llenguatge**: Català/Valencià

## Instal·lació i ús local

### Requisits

- Python 3.x
- pip

### Passos

1. Clona el repositori:
```bash
git clone https://github.com/arturocandela/blog.git
cd blog
```

2. Instal·la les dependències:
```bash
pip install mkdocs mkdocs-material
```

3. Executa el servidor de desenvolupament:
```bash
mkdocs serve
```

4. Obri el navegador a `http://127.0.0.1:8000/blog/`

## Desplegar

El blog es desplega automàticament a GitHub Pages. Per desplegar manualment:

```bash
mkdocs gh-deploy
```

Això construeix el lloc i el publica a la branca `gh-pages`.

## Estructura del projecte

```
blog/
├── docs/                  # Contingut del blog
│   ├── index.md          # Pàgina principal
│   └── posts/            # Entrades del blog
├── mkdocs.yml            # Configuració de MkDocs
├── agents.md             # Política d'ús d'agents d'IA
└── README.md             # Aquest fitxer
```

## Contribució i política de commits

Aquest és un projecte personal, però si vols suggerir millores o correccions, obre un issue.

⚠️ **Important**: Consulta [agents.md](agents.md) per conèixer la política sobre l'ús d'agents d'IA i commits en aquest repositori. **Els commits no poden incloure co-autoria amb agents d'IA**.

## Autor

**Arturo Candela**

- GitHub: [@arturocandela](https://github.com/arturocandela)
- Blog: [arturocandela.github.io/blog](https://arturocandela.github.io/blog/)

## Llicència

El contingut d'aquest blog és propietat d'Arturo Candela. El codi està disponible amb finalitats educatives.

---

*Última actualització: Febrer 2026*
