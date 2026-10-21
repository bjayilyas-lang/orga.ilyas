# Doucement — Organiseur de projets

Petit site responsive en HTML, CSS et JavaScript, sans installation ni compilation. Il comporte quatre pages : accueil, création/modification de projet, planning avec calendrier mensuel et historique.

## Utilisation
1. Décompresse le dossier et ouvre `index.html` dans un navigateur, ou publie les fichiers sur un hébergement statique (GitHub Pages, Netlify ou Vercel).
2. Crée un projet et ajoute des tâches avec dates, heures, durées, descriptions et, si besoin, une adresse. L'adresse est facultative.
3. Le site refuse l'enregistrement si deux tâches non terminées se chevauchent sur un même créneau, y compris entre projets actifs. Les tâches sans date ou sans heure ne sont pas prises en compte dans ce contrôle.
4. Dans le planning, choisis le délai des notifications du navigateur (à l'heure, 5, 10, 15, 30, 45 minutes, 1, 2 ou 24 heures avant). Autorise les notifications lorsque le navigateur le demande. Elles ne fonctionnent que lorsque le site est ouvert et actif ; ce n'est pas un système d'alerte garanti en arrière-plan.
5. Dans le planning, les tâches avec une adresse apparaissent dans l'ordre de l'heure. Saisis un point de départ et, si besoin, une destination finale, puis clique sur **Générer le trajet en voiture**. Une carte OpenStreetMap affiche le trajet routier calculé par OSRM, et le parcours s'ouvre aussi dans Google Maps.
6. Clique sur l'icône ↗ d'une tâche datée pour télécharger un fichier `.ics` importable dans Apple Calendar, Google Calendar ou Outlook. Le délai d'alerte du fichier calendrier reprend le réglage choisi dans le planning.
7. Les données sont enregistrées dans le `localStorage` du navigateur. Elles ne se synchronisent pas automatiquement entre appareils : ajoute une base de données si tu souhaites une synchronisation.

## Limites à connaître
- La carte intégrée utilise Leaflet, les tuiles OpenStreetMap, le géocodage Nominatim et le calcul d'itinéraire OSRM. Ces services publics peuvent être indisponibles ou limités ; dans ce cas, le lien Google Maps reste proposé. Les adresses sont envoyées à ces services externes au moment de générer la carte.
- Le site statique ne peut pas envoyer de courriels de lui-même. Pour des e-mails automatiques avant une tâche, il faut ajouter un service côté serveur ou une automatisation, une base de données et un fournisseur d'e-mail.
- Les notifications du navigateur dépendent de l'autorisation accordée et du fait que le site reste ouvert. Pour des rappels plus fiables, importe les tâches dans le calendrier de ton téléphone ou de ton ordinateur.

## Mise en ligne rapide
- **Netlify** : glisse le dossier du site dans Netlify Drop.
- **Vercel** : importe le dossier/dépôt en tant que site statique, sans commande de build.
- **GitHub Pages** : pousse les fichiers dans un dépôt puis active Pages.

Le site utilise Google Fonts si une connexion Internet est disponible, mais reste fonctionnel sans elles.
