# Cycle de vie d'une requête Laravel

Lorsqu'un utilisateur visite la page `/heure` :

1. Le navigateur envoie une requête HTTP vers Laravel.
2. Le fichier `public/index.php` reçoit la requête.
3. Le fichier `vendor/autoload.php` charge les classes nécessaires.
4. Le fichier `bootstrap/app.php` initialise l'application Laravel.
5. Laravel consulte les routes définies dans `routes/web.php`.
6. Laravel trouve la route `/heure` et exécute sa fonction.
7. La fonction appelle la vue `resources/views/heure.blade.php`.
8. Blade génère le code HTML contenant l'heure et la date.
9. Laravel renvoie la réponse HTML au navigateur.