## Connexion à Instagram

1. Dans votre client Matrix, ouvrez une discussion privée avec `@__BOTNAME__:__SERVER_NAME__` (si le compte n'apparaît pas dans l'annuaire, tapez l'identifiant complet).
2. Envoyez `login instagram`. Le robot demande vos cookies instagram.com, sous forme d'objet JSON ou de commande cURL.
3. Dans un navigateur de bureau connecté à instagram.com, ouvrez les outils de développement (`F12` ou `Cmd+Option+I`) → onglet **Réseau**, rechargez la page, clic droit sur une requête vers `www.instagram.com` → **Copier** → **Copier en tant que cURL**, et collez le résultat en réponse au robot.
4. Une fois connecté, vos conversations apparaissent comme des salons Matrix. Supprimez de la discussion le message contenant les cookies, et **ne vous déconnectez pas** d'instagram.com dans ce navigateur (cela invaliderait la session).

Commandes utiles (dans la discussion avec le robot) : `help`, `list-logins`, `logout <ID de connexion>`.

En cas de problème : `sudo yunohost service log __APP__` ou `/var/log/__APP__/__APP__.log`.
