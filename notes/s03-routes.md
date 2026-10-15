# Session 03 - Routes, contrôleurs et layout

## Défi

URL produite par route('about') : route('about') : http://localhost:8000/a-propos

URL produite par route('posts.show', 'routes-et-controleurs') : route('posts.show', 'routes-et-controleurs') : http://localhost:8000/posts/routes-et-controleurs

URL produite par route('posts.archive', 2025) : route('posts.archive', 2025) : http://localhost:8000/posts/archive/2025

Pourquoi /posts/archive/abc et /posts/article-inconnu répondent toutes deux 404, et quelle ligne de code en est responsable dans chaque cas ?  

/posts/archive/abc : whereNumber('year') dans web.php rejette la route. /posts/article-inconnu : la route correspond, puis abort(404) dans PostController::show répond 404.

Que se passe-t-il si une vue appelle route('posts.show') sans paramètre ? 
Laravel affiche l'erreur Missing required parameter for [Route: posts.show].