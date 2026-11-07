# Publication du site ORACULUM

La page du site est dans [index.html](index.html). Le workflow GitHub Actions est prêt dans `.github/workflows/pages.yml`.

## Activer GitHub Pages

Dans le dépôt, ouvre **Settings → Pages**, puis dans **Build and deployment → Source**, choisis **GitHub Actions**. Le site sera ensuite publié automatiquement après un envoi sur la branche `main`.

L'adresse prévue est : https://la-fondation-oraculum.github.io/ORACULUM/

## Publier les fichiers de jeu

La page attend les fichiers suivants dans une Release GitHub publique :

- `ORACULUM-Android-1.1.0-debug.apk`
- `ORACULUM-Linux-1.1.2-all.deb`
- `ORACULUM-Linux-1.1.2.tar.gz`

La page fabrique les liens `releases/latest/download/NOM_DU_FICHIER`. Les paquets ne sont pas stockés dans le dépôt : il faut les joindre à une Release GitHub pour activer les téléchargements. La connexion GitHub utilisée ici permet de mettre à jour les fichiers du dépôt, mais pas de téléverser les binaires sur une Release. Ajoute les fichiers dans **Releases → Draft a new release → Attach binaries**.

Les fichiers Linux 1.1.2 sont disponibles localement dans `outputs/ORACULUM_VERSION_SUIVANTE` : `ORACULUM-Linux-1.1.2-all.deb` et `ORACULUM-Linux-1.1.2.tar.gz`. L’APK Android référencé sur le site est `ORACULUM-Android-1.1.0-debug.apk`.
