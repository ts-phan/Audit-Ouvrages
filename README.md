# Audit Ouvrages — PWA v17

Application web terrain pour l'audit d'ouvrages.
Fonctionne hors-ligne sur iPhone et Android (installable comme app).

## Gestes mobiles

| Geste | Action |
|-------|--------|
| ☝️ Toucher court (< 280 ms) | Poser une annotation (mode 📍) |
| 👆 Glisser 1 doigt | Naviguer / déplacer le plan (tous modes) |
| 🤏 Pincer / écarter 2 doigts | Zoom |

## Structure du dépôt

```
├── index.html        — Page principale
├── style.css         — Styles
├── app.js            — Logique (obfusquée)
├── sw.js             — Service Worker (mode hors-ligne)
├── manifest.json     — Manifest PWA
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## Déploiement GitHub Pages

1. Renommer `gitignore.txt` → `.gitignore`
2. `git init && git add . && git commit -m "Deploy PWA"`
3. `git remote add origin https://github.com/USER/REPO.git && git push -u origin main`
4. GitHub → Settings → Pages → Source : `main / root`

URL : `https://USER.github.io/REPO/`

## Installation sur téléphone

**iPhone (Safari)** → Partager → "Sur l'écran d'accueil"
**Android (Chrome)** → Menu ⋮ → "Ajouter à l'écran d'accueil"
