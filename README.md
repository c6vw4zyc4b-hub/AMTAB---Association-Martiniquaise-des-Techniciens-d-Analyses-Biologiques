# Site AMTAB

Site vitrine de l'Association Martiniquaise des Techniciens d'Analyses Biologiques.

## Fichiers

- `index.html` — page principale (accueil, qui sommes-nous, actualités, annonces, adhésion, contact)
- `actualites.html` — page listant l'intégralité des articles d'actualité
- `.nojekyll` — fichier technique demandant à GitHub Pages de servir les fichiers tels quels

## Mettre le site en ligne avec GitHub Pages

1. Créez un dépôt GitHub (public, pour que GitHub Pages soit gratuit).
2. Déposez-y ces fichiers (`index.html`, `actualites.html`, `.nojekyll`) à la racine du dépôt.
3. Dans le dépôt, allez dans **Settings** → **Pages**.
4. Sous **Build and deployment**, choisissez la source **Deploy from a branch**, sélectionnez la branche `main` (ou `master`) et le dossier `/ (root)`, puis cliquez sur **Save**.
5. Après une à deux minutes, le site est accessible à une adresse du type :
   `https://votre-nom-utilisateur.github.io/nom-du-depot/`

## Utiliser un nom de domaine personnalisé (optionnel)

Si vous possédez un nom de domaine (ex. amtab-martinique.fr) :

1. Dans **Settings** → **Pages**, renseignez-le dans le champ **Custom domain**.
2. Chez votre registrar (OVH, Gandi...), ajoutez les enregistrements DNS demandés par GitHub (en général un enregistrement `CNAME` pointant vers `votre-nom-utilisateur.github.io`, ou des enregistrements `A` pour les adresses IP de GitHub Pages).
3. Attendez la propagation DNS, puis cochez **Enforce HTTPS** une fois le certificat généré.

## Mettre à jour le site plus tard

Remplacez simplement `index.html` et/ou `actualites.html` par leur nouvelle version dans le dépôt (via l'interface web de GitHub — bouton "Add file" → "Upload files" — ou via `git push`). Le site se met à jour automatiquement en une à deux minutes.
