# Diorite Studio — site vitrine

Landing page de Diorite Studio : publicités Facebook & Instagram locales pour les artisans du bâtiment.

En ligne : https://arthursynkore.github.io/granit/ (GitHub Pages, branche `main`, dossier racine).

## Structure

```
index.html              page d'accueil (VSL, méthode, garantie, résultats, FAQ, agenda Calendly, WhatsApp)
mentions-legales.html   mentions légales (obligatoires)
confidentialite.html    politique de confidentialité (RGPD)
404.html                page introuvable
robots.txt, sitemap.xml référencement
assets/
  style.css             toute la mise en forme (charte : diorite claire, ardoise, jaune chantier)
  fonts/                polices hébergées sur le site (Barlow Condensed, Public Sans, IBM Plex Mono)
  diorite-vsl.mp4       vidéo de présentation (26 s)
  vsl-cover.jpg         image affichée avant lecture
  og-image.jpg          aperçu quand le lien est partagé (WhatsApp, LinkedIn, Facebook…)
  diorite-studio-logo*.svg, favicon.svg, apple-touch-icon.png, icon-512.png
```

## Modifier le site

- Textes : directement dans `index.html`.
- Couleurs / typos : variables en haut de `assets/style.css`.
- Agenda : lien Calendly dans la section `#agenda` de `index.html`.
- WhatsApp : numéro dans les liens `wa.me/33662013243`.

## Passer sur un vrai nom de domaine

1. Acheter le domaine (ex. chez OVHcloud pour un `.fr`).
2. Dans la zone DNS du domaine, ajouter :
   - 4 enregistrements `A` sur `@` : `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - 1 enregistrement `CNAME` sur `www` → `arthursynkore.github.io.`
3. Sur GitHub : *Settings → Pages → Custom domain* → saisir le domaine, puis cocher *Enforce HTTPS*.
4. Remplacer `https://arthursynkore.github.io/granit/` par le nouveau domaine dans `index.html`, les pages légales, `robots.txt` et `sitemap.xml`, et remplacer `/granit/` par `/` dans `404.html`.
