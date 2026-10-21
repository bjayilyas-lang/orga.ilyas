# Notre 1 an — Organiseur

Petit site statique (HTML / CSS / JS, aucune dépendance, aucun build) pour organiser les tâches de l'anniversaire : date, heure, catégorie, priorité, compte à rebours et rappel via l'agenda du téléphone.

Les données sont stockées dans le navigateur (`localStorage`). Utilise **Exporter** de temps en temps pour garder une sauvegarde.

## Mettre en ligne

### 1. GitHub
1. Crée un dépôt vide sur github.com (ex. `organiseur`).
2. Dans ce dossier :
   ```bash
   git init
   git add .
   git commit -m "Premier commit"
   git branch -M main
   git remote add origin https://github.com/TON-COMPTE/organiseur.git
   git push -u origin main
   ```

### 2. Vercel
1. Sur vercel.com : **Add New → Project** puis importe le dépôt GitHub.
2. Ne change rien (Framework Preset : *Other*, pas de build command, pas d'output directory).
3. **Deploy**. Le site est en ligne sur `https://organiseur-xxxx.vercel.app`.

Sur le téléphone, ouvre le lien puis « Ajouter à l'écran d'accueil » pour l'avoir comme une appli.

> Chaque navigateur/appareil a ses propres données : utilise toujours le même appareil, ou passe par Exporter / Importer.
