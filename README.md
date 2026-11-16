# Arthur Maire — CV

Site CV statique, en français et adapté aux écrans mobiles et desktop. Les coordonnées personnelles du CV source ne sont pas publiées.

## Prévisualisation locale

Ouvrir `index.html` dans un navigateur. Le site n’a pas de dépendance ni d’étape de compilation. Le dossier `doc/` contenant le CV source est ignoré par Git.

## Déploiement sur GitHub Pages

Le workflow `.github/workflows/pages.yml` déploie automatiquement le site lors d’un push sur `main`. Il ne publie que `index.html` et `styles.css` ; le CV source dans `doc/` n’est ni versionné ni inclus dans le site.

1. Créer un dépôt GitHub et y envoyer la branche `main` :

   ```sh
   git remote add origin https://github.com/<utilisateur>/<depot>.git
   git push -u origin main
   ```

2. Dans le dépôt GitHub, ouvrir **Settings → Pages**, puis choisir **GitHub Actions** comme source de déploiement.
3. Vérifier l’exécution du workflow dans l’onglet **Actions**. L’adresse publique du site sera indiquée dans l’environnement `github-pages` et dans les détails du déploiement.

Le déploiement automatique ne démarre qu’après l’ajout d’un dépôt distant GitHub et l’activation de GitHub Pages.
