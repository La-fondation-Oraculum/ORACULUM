# Publication du site ORACULUM

La page du site est dans [index.html](index.html). Le workflow GitHub Actions est prêt dans `.github/workflows/pages.yml`.

## Activer GitHub Pages

Dans le dépôt, ouvre **Settings → Pages**, puis dans **Build and deployment → Source**, choisis **GitHub Actions**. Le site sera ensuite publié automatiquement après un envoi sur la branche `main`.

L'adresse prévue est : https://la-fondation-oraculum.github.io/ORACULUM/

## Publier les fichiers de jeu

La page attend les fichiers suivants dans une Release GitHub publique :

- `ORACULUM-Android-1.1.0-debug.apk`
- `ORACULUM-Linux-1.1.0-all.deb`
- `ORACULUM-Linux-1.1.0.tar.gz`

La page fabrique les liens `releases/latest/download/NOM_DU_FICHIER`. Les paquets ne sont pas dans le dépôt et ne sont pas encore attachés à une Release. La connexion GitHub utilisée ici ne propose pas l'API de création de Release ni le téléversement des assets ; ces trois fichiers devront être ajoutés dans l'interface GitHub : **Releases → Draft a new release → Attach binaries**.

Les fichiers sont disponibles localement dans le dossier de livraison `outputs/ORACULUM_VERSION_SUIVANTE`.
