# Radio Fleurs de Dieu — Site web

Site officiel de Radio Fleurs de Dieu (RFDD), radio chrétienne adventiste en ligne.

## Fichiers

- `index.html` — page d'accueil (lecteur live + programmes + nouvelles + donation)
- `don.html` — page de donation (lien Stripe)
- `assets/logo.jpeg` — logo de la radio

## Mettre en ligne sur GitHub Pages (gratuit)

1. Crée un compte sur https://github.com (si ce n'est pas déjà fait).
2. Crée un nouveau dépôt (repository) public, par exemple nommé `radio-fleurs-de-dieu`.
3. Téléverse les 3 fichiers/dossiers : `index.html`, `don.html`, et le dossier `assets/`.
4. Dans le dépôt : **Settings → Pages**.
5. Sous "Branch", choisis `main` et le dossier `/ (root)`, puis **Save**.
6. Après 1-2 minutes, ton site sera en ligne à l'adresse :
   `https://TON-COMPTE.github.io/radio-fleurs-de-dieu/`

## Points à mettre à jour

### 1. Lien de don Stripe (IMPORTANT)
Le lien actuel est un lien **de TEST** :
`https://buy.stripe.com/test_8x23cveQe1Eu8Z505qa3u00`

Quand le compte Stripe sera vérifié (bouton « Vérifier votre entreprise ») et le compte
bancaire connecté, crée le **vrai** lien de paiement (sans « test_ » dans l'URL), puis
remplace l'adresse dans `don.html` (cherche `buy.stripe.com`) — il y a 1 seul endroit.

### 2. Stream Zeno.fm
Le lecteur utilise : `https://stream.zeno.fm/wsm8528kuhruv`
Si l'URL du stream change un jour, remplace-la dans `index.html` (2 endroits :
la balise `<source>` et la ligne `audio.src` dans le script).

## Domaine personnalisé (optionnel, plus tard)
Pour utiliser un domaine comme `radiofleursdedieu.org` :
achète le domaine, puis dans **Settings → Pages → Custom domain**, entre-le et
configure les DNS chez ton registraire (GitHub donne les instructions).
