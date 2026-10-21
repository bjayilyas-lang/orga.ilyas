# Doucement — maquette avancée

## Installation sur GitHub Pages
1. Téléchargez et décompressez l'archive.
2. Importez **tout le contenu** du dossier dans la racine du dépôt GitHub (les fichiers HTML doivent être au même niveau que `styles.css` et `app.js`).
3. Dans GitHub : **Settings → Pages**, sélectionnez la branche principale et le dossier `/ (root)`.
4. Attendez la publication puis ouvrez l'URL fournie par GitHub Pages.

## Modules inclus
- `index.html` : accueil et rituel quotidien
- `souvenirs.html` : souvenirs
- `idees.html` : idées à faire ensemble
- `journee.html` : journée spéciale et calendrier
- `budget.html` : budget, opérations et graphique
- `voyages.html` : recherche de lieux, carte OpenStreetMap et étapes de voyage
- `messages.html` : messages à ouvrir
- `stats.html` : statistiques
- `planning.html` : planning

## À savoir avant publication
- Cette livraison est une **maquette front-end fonctionnelle**, pas encore une application multi-utilisateur de production.
- Les données sont enregistrées dans le `localStorage` du navigateur. Elles ne sont pas synchronisées entre appareils et ne sont pas partagées avec l'ancien site automatiquement.
- Aucune base Supabase n'est connectée dans cette archive. Pour synchroniser à deux, il faudra créer/configurer Supabase, ajouter l'authentification et brancher les opérations de lecture/écriture.
- Les polices et certaines images sont chargées depuis Internet. La carte et la recherche de lieux nécessitent également une connexion Internet.
- Avant de remplacer le site actuel, conservez une copie de sauvegarde de ses fichiers et de ses données.
