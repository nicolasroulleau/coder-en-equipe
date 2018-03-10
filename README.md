# ATELIER DU 9 mars 2018 - coder-en-equipe

Problématique: le code vit
Code qui existe avant nous: code legacy
Toujours coder avec l'objectif qu'un octogénaire sache s'en servir
Le code doit refléter le métier: nom des modèles, des méthodes, des variables.
Bonnes pratiques:
- commenter son code
- naming conventions: variable en minuscule, Classe avec une majuscule, CONSTANTE en majuscule
Outils de collaboration:
- gestion des versions
- gestion des tâches (Trello, Pivotal Tracker, Jira (horrible))
Les Stories dans Trello doivent être purement fonctionnelles ex: j'arrive à me login
Ensuite découpage technique
NB: normalement il faut utiliser un autre model pour l'admin (rails g devise:admin)

Git permet de remonter le temps donc pas besoin de laisser du code mort
git-flow-cheatsheet (ne pas utiliser l'outil gitflow mais seulement la méthode)
10 commandes de base git: 
git status
git checkout -b (cool-feature)
git push (origin cool-feature) attention la nouvelle branche n'a pas été créée à distance
git add ### (jamais faire git add .)
git commit -m "######"
git checkout master
git pull --prune (pour virer en local toutes les branches qui ont été virées à distance) => toujours pull depuis master
NB: ne jamais jouer avec une BDD de prod et l'arbre git
git checkout - (- signifie précédent) pour revenir sur ma branche
git merge master => je merge la branche master à ma branche
je teste avec un rails s

GitLab a le CI gratuit (serveur de continuous integration) pour faire tourner les tests

Tests recommandés: tests unitaires => TDD sur un modèle
Fat models skinny controllers 
dès qu'une méthode touche à la BDD, on la met dans les modèles

##Ruby naming conventions



