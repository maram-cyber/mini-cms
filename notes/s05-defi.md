# Session 05 - Défi : articles récents sur l'accueil

latestPosts contient au plus 3 articles : oui
Seuls les articles publiés sont transmis à la vue : oui 
home.blade.php utilise x-post-card et @forelse : oui 
Le nouveau test passe et php artisan test est vert : oui 

Pourquoi get() et pas paginate(3) sur la page d'accueil ?
get() récupère les articles correspondant à la requête. Avec limit(3)->get(), tu récupères au maximum 3 articles, sans pagination.



paginate(3) récupère 3 articles par page et prépare les liens de pagination (page suivante, page précédente).