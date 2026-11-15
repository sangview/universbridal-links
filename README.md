# links.universbridal.com

Page de liens Univers Bridal (réseaux sociaux + contact WhatsApp direct). Site statique : `index.html`, `favicon.svg`, `CNAME`.

## Modifier les liens

Ouvrez `index.html` et éditez le bloc **`PROFILE`** (repéré par « ✏️ À MODIFIER ») :

- `whatsapp.number` : numéro au format international, chiffres uniquement (06 12 34 56 78 → `33612345678`)
- `whatsapp.message` : message pré-rempli à l'ouverture de la conversation
- `links` : un réseau par ligne ; supprimez une ligne pour le masquer. Icônes disponibles : `instagram`, `tiktok`, `facebook`, `pinterest`, `youtube`, `globe`, `mail`

Logo : déposez `logo.jpg` à côté de `index.html` et remplacez `<span class="monogram">UB</span>` par `<img src="logo.jpg" alt="">`.

## Mise en ligne (gratuite) — au choix

### Option A : Netlify / Cloudflare Pages (le plus simple)
1. Glissez-déposez ce dossier sur https://app.netlify.com/drop (ou créez un projet Cloudflare Pages).
2. Dans les réglages du site → *Domaines* → ajoutez `links.universbridal.com`.
3. Chez votre registrar (là où universbridal.com est géré), créez l'enregistrement DNS indiqué :
   `CNAME  links  →  <votre-site>.netlify.app` (ou `<projet>.pages.dev`).
4. Le HTTPS s'active automatiquement en quelques minutes.

### Option B : GitHub Pages
1. Poussez ce dossier dans un dépôt GitHub, puis *Settings → Pages → Deploy from branch (main, /root)*.
2. Le fichier `CNAME` déclare déjà le domaine `links.universbridal.com`.
3. DNS : `CNAME  links  →  <votre-utilisateur>.github.io`, puis cochez *Enforce HTTPS*.

## Aperçu local

```bash
python -m http.server 4173
```
puis ouvrez http://localhost:4173
