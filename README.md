# Coaching Présentiel — Tunnel Webinaire

Tunnel d'inscription pour le webinaire « Retrouver votre énergie (sans vous épuiser) »,
menant vers le programme de coaching présentiel 13 semaines de Stéphane Amourda.

## Fichiers

- `index.html` — Page d'inscription (opt-in) au webinaire.
- `merci.html` — Page de remerciement après inscription.

## Configuration avant mise en ligne

Dans `index.html`, section `<script>` en bas de page, renseigner :

```js
const CONFIG = {
  SYSTEME_IO_URL: "https://xxxx.systeme.io/inscription-webinaire", // ton URL Systeme.io
  FIELD_NAMES: { firstName: "prenom", email: "email" }
};
```

Dans `merci.html`, une fois la date du webinaire fixée :

```js
const CONFIG = {
  WEBINAR_DATE_ISO: "2026-09-15T13:00:00", // date et heure réelles
  REGISTRATION_LINK: "https://tonlien.fr/webinaire" // une fois la page en ligne
};
```

## Hébergement (GitHub Pages)

1. Aller dans **Settings > Pages** de ce dépôt.
2. Source : `Deploy from a branch`, branche `main`, dossier `/ (root)`.
3. La page sera accessible à `https://stephane-amourda.github.io/Coaching-presentiel/`.
