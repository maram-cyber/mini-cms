# Session 02 - Git et GitHub

Réponses rédigées avec mes propres mots, puis comparées au corrigé de la page.

## 1. Index et commit

Réponse :git add (du répertoire de travail vers l'index), git commit (de l'index vers le dépôt local) ; git push envoie ensuite au dépôt distant

## 2. Branche et tag

Réponse :Une branche avance à chaque commit ; un tag reste fixé sur un commit (lab-01 désigne toujours la fin de la session 01)

## 3. Le fichier .env

Réponse :.env contient APP_KEY et les réglages propres au poste (et des secrets en production). On copie .env.example puis on lance php artisan key:generate.

## 4. Le dossier vendor/

Réponse :vendor/ est volumineux et entièrement généré ; composer install le reconstruit avec les versions exactes de composer.lock.

## 5. Git Credential Manager

Réponse :Dans le Gestionnaire d'identification Windows (entrée git:https://github.com). On le supprime sur un poste de l'université, car la personne suivante pourrait pousser en votre nom ; on le garde sur son ordinateur personnel.
## 6. Historique depuis lab-01

Nombre de commits depuis lab-01 : Nombre de commits : 5 avant ce dernier commit (6 si le commit « Completer le travail de la session 01 » existe).

Fichiers modifiés depuis lab-01 : Fichiers modifiés : les 5 fichiers listés à l'Étape 7 (notes/s02-git.md, routes/web.php, resources/views/a-propos.blade.php, screenshots/s02-a-propos.png, README.md), README.md ayant été modifié une deuxième fois par la partie 1, plus les fichiers éventuels du commit « Completer le travail de la session 01 ».

Ce que git tag -n affiche pour lab-01 : git tag -n : lab-01 suivi du message du commit qu'il désigne (lab-01).