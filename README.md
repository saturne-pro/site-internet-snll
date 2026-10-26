# Site internet — Transports SNLL

Site vitrine de Transports SNLL (Cergy), conçu par Saturne Pro.

## Contenu
- `index.html` — le site (8 pages : accueil, services, réservation, à propos, recrutement, contact, espace client, mentions légales)
- `support.js` — moteur de rendu du site
- `assets/` — visuels

## Lancer en local
```bash
npx serve .
```
Puis ouvrir http://localhost:3000

## Version de travail (GitHub Pages)
Le site est publié automatiquement sur https://saturne-pro.github.io/site-internet-snll/
à chaque push (workflow `.github/workflows/pages.yml`).

## Avant mise en production
- Retirer la balise `<meta name="robots" content="noindex, nofollow">` et le badge « Maquette · version de travail » (`.snll-draft`)
- Remplacer les données de démonstration (téléphone, e-mail, chiffres, témoignages, tarifs, équipe)
- Brancher les formulaires sur une API sécurisée (HTTPS, CSRF, rate limiting, validation serveur)
- Configurer les en-têtes de sécurité (CSP, HSTS, X-Content-Type-Options, Referrer-Policy)
- Remplacer les illustrations par les photos réelles
