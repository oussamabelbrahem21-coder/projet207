# Peugeot 207 Dashboard - application Android

Deux façons d'installer, choisis la plus simple pour toi.

## Option A - APK (recommandé pour un écran de voiture)

Je n'ai pas d'Android SDK ici, donc l'APK se génère gratuitement en ligne (environ 5 min, sans rien installer) :

1. Crée un compte sur https://github.com (gratuit).
2. Nouveau dépôt (New repository), nom : `projet207`, public ou privé.
3. Clique « uploading an existing file » et glisse **tout le contenu** de ce dossier
   (dossiers `app`, `.github`, `pwa` + fichiers `build.gradle`, `settings.gradle`, `gradle.properties`).
   Attention : le dossier `.github` est caché sur certains systèmes, active « afficher les fichiers cachés ».
4. Clique « Commit changes ».
5. Onglet **Actions** > « Build APK » > attends la coche verte (si rien ne démarre : « Run workflow »).
6. Clique sur la build > en bas, **Artifacts > Projet207-APK** > télécharge le zip > dedans : `app-debug.apk`.
7. Copie l'APK sur clé USB ou envoie-le sur le téléphone, puis installe-le sur l'autoradio
   (autorise « sources inconnues » si demandé).

Au premier lancement, accepte l'autorisation de **localisation** (pour la navigation/GPS).

## Option B - PWA (pas d'APK)

Dossier `pwa/` : héberge-le en HTTPS (ex. https://app.netlify.com/drop : glisse le dossier),
ouvre l'adresse dans Chrome sur l'autoradio > menu > « Installer l'application ».
Fonctionne ensuite hors ligne (sauf cartes et recherche d'adresse, qui ont besoin d'internet).

## Notes
- Plein écran, orientation paysage, écran toujours allumé, bouton retour ignoré (pour ne pas quitter par erreur).
- Android 5.0 minimum.
- Le fichier HTML d'origine est inchangé (`app/src/main/assets/index.html`).
