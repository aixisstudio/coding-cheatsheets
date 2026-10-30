# Coding Cheatsheets

[English](README.md) | **Français** | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Des antisèches de dev qui servent vraiment

Les draps de chauffage qui sont utilisés

♪ ♪ ♪ Git

Qu'est-ce qui se passe ?
|---|---|
`git log --oneline --graph --all`? Visualiser les branches
`git stash && git stash pop`?Parc + restauration
Démonter le dernier commit, conserver les modifications
Réécrire les 3 derniers commits
`git bisect start`= Recherche binaire dans le commit de bogue
Le sauveur de vie Undo-undo
Enlever les fichiers non suivis

Coquille

Qu'est-ce qui se passe ?
|---|---|
`cmd1 && cmd2`. Exécuter 2 seulement si 1 réussit.
Imprimer et enregistrer la sortie
`cmd > out 2>&1`=Rediriger le stderr vers stdout=
`Ctrl-A / Ctrl-E`=Démarrage de la ligne / fin
Ré-exécuter la dernière commande correspondante
Loop sur les fichiers

La boucle

Qu'est-ce qui se passe ?
|---|---|
Rechercher + parse JSON
`curl -X POST -d '{"a":1}' -H 'Content-Type: json'`
Téléchargement
`curl -v url`
`curl --retry 5 url`: Réessayer automatiquement

Python monoligne

Quoi ?
|---|---|
Serveur de fichiers instantanés
`python3 -m json.tool < data.json`? Jolie impression JSON?
Compréhension de la liste
`dict(zip(keys, vals))`: Zip pour dicter

Vite !

Qu'est-ce qui se passe ?
|---|---|
Qu'est-ce qui t'écoute
TLS poignée de main debug
Couverture MD5
John l'Éventreur
`shasum -a 256 file`

# # # # C'est Docker

Qu'est-ce qui se passe ?
|---|---|
Tous les conteneurs
`docker exec -it c bash`
`docker logs -f c`
`docker system prune -af`
Utilisation des ressources en direct
Contenant éphémère

J'ai avancé Git

Qu'est-ce qui se passe ?
|---|---|
Deuxième commande, même repo
`git cherry-pick abc123`
Renommer
`git diff main...feature`
`git commit --fixup abc && git rebase -i --autosquash`= Correction de l'historique propre
Une force plus sûre

Les superpuissances

Qu'est-ce qui se passe ?
|---|---|
Recherche filtrée par type
Nombre de fichiers avec TODOS
Contexte après match
Fichiers manquants

"Régex"

Modèle correspondant
|---|---|
Après @ (regarder)
`\w+@\w+\.\w+`: Courriels
Adresses IPv4
`(?=.*[A-Z])(?=.*\d).{8,}`=Validateur de mot de passe

# # # , , SQLite

Qu'est-ce qui se passe ?
|---|---|
Liste des tableaux
Tableau DDL
Sortie lisible
`.dump`=Exporter tout

---
## Contribuer

Les pull requests sont les bienvenues : ouvre une PR, elle sera relue et fusionnée. Maintenu par [aixisstudio](https://github.com/aixisstudio), auteur de [Snitch](https://github.com/aixisstudio/Snitch), pare-feu applicatif open source.

## Licence: MIT
