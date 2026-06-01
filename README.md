# Audit Ouvrages — PWA

Application web terrain pour l'audit d'ouvrages.  
Fonctionne hors-ligne sur iPhone et Android (installable comme app).

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

## Installation sur téléphone

### Android (Chrome)
1. Ouvrir l'URL GitHub Pages dans Chrome
2. Menu ⋮ → "Ajouter à l'écran d'accueil"

### iPhone (Safari)
1. Ouvrir l'URL GitHub Pages dans Safari
2. Bouton Partager → "Sur l'écran d'accueil"

## Déploiement GitHub Pages

1. Pousser ce dépôt sur GitHub
2. Settings → Pages → Source : `main` / `root`
3. L'URL sera : `https://<username>.github.io/<repo>/`

## Mise à jour du cache PWA

Incrémenter `CACHE_NAME` dans `sw.js` à chaque nouvelle version.
# Audit-Ouvrages
