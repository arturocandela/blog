# Agents i assistents

Aquest document descriu l'ús d'agents d'IA en aquest repositori.

## Sobre aquest repositori

Aquest és el **blog personal d'Arturo Candela**, un espai per compartir idees, proves i aprenentatges sobre tecnologia i desenvolupament de software.

- **Plataforma**: MkDocs amb el tema Material
- **Allotjament**: GitHub Pages
- **URL**: https://arturocandela.github.io/blog/
- **Contingut**: Notes de projectes personals, aprenentatges tècnics, entrades curtes amb proves i experiments

## Ús d'agents

En el desenvolupament d'aquest blog es poden utilitzar diversos agents d'IA (com Claude, assistents de programació, etc.) per:

- Ajudar amb la generació de codi
- Revisar i millorar contingut
- Automatitzar tasques repetitives
- Resoldre problemes tècnics

## Política de commits

**IMPORTANT**: Quan es faça un commit en aquest repositori, **NO pot estar coescrit amb cap agent**.

Els commits han de reflectir l'autoria humana i no incloure línies com:

```
Co-Authored-By: Claude <noreply@anthropic.com>
Co-Authored-By: [qualsevol agent d'IA]
```

### Raó

Els agents són eines d'assistència, però l'autoria i responsabilitat del contingut i codi és exclusivament humana. Els commits han de reflectir aquesta realitat.

### Configuració

Quan utilitzes agents per ajudar-te amb el codi, assegura't que:

1. Els missatges de commit no incloguen co-autoria amb agents
2. Revises i entens tots els canvis abans de fer commit
3. Assumes la responsabilitat total del contingut publicat

## Directrius de Commit i Pull Request

### Format dels missatges de commit

Anteposar als títols dels commits una etiqueta que categoritza el canvi:

- **[MOD]** – Modificació de codi o arxius existents
- **[ADD]** – Addició de nous arxius o funcionalitats
- **[DEL]** – Eliminació d'arxius o codi
- **[FIX]** – Correcció d'errors o bugs

### Bones pràctiques

1. **Títol imperatiu i específic**: Escriure el títol després de l'etiqueta en mode imperatiu i específic
   - ✅ `[ADD] Exportació de calendari a esdeveniments`
   - ✅ `[FIX] Punter nul en login d'usuari`

2. **Mantenir canvis relacionats junts**: Agrupar els canvis relacionats en el mateix commit

3. **Verificar issues abans de fer commit**: Abans de confirmar els canvis, comprovar si hi ha issues relacionades a GitHub:
   ```bash
   gh issue list
   gh issue status
   ```

4. **Referenciar issues**: Si els canvis aborden o es relacionen amb una issue, referenciar-la en el missatge de commit utilitzant `#numero_issue`
   - ✅ `[FIX] Punter nul en login d'usuari #42`
   - ✅ `[MOD] Refactorització del flux d'autenticació #15 #23`

5. **No incloure co-autoria amb IA**: Els missatges de commit **no** han d'incloure `Co-Authored-By: Claude` o atribucions similars a agents d'IA

---

*Última actualització: 14 de febrer de 2026*
