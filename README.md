![separe](https://github.com/studoo-app/.github/blob/main/profile/studoo-banner-logo.png)
# Go - CLI de génération de mots de passe avec Cobra-Cli
[![Version](https://img.shields.io/badge/Version-2025-blue)]()

## Objectifs

Créer une CLI permettant de générer des mots de passes, il devra être possible de générer des mots de passes pour contenir 
ou non des chiffres et/ou des caractères spéciaux.

## Build

Exécuter la commande suivante dans le terminal du container dev-server

```bash
go build
```

## Déploiement dans le serveur de test

Copier l'éxécutable générer dans le dossier `/share`, ensuite se connecter au terminal du test-server et déplacer ce dernier
dans le dossier `/usr/bin` afin de rendre la commande disponible.

```bash
mv /root/share/pwdGen /usr/bin/pwdGen
```

## Test de la commande

```bash
pwdGen generate -l 12 -d -s
```