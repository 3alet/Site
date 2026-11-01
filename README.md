# Haut Risque — code complet du site

Version exportée le 1 novembre 2026, commit 331056a05e114eb06d430a470d258e5003d9595f.

## Ouvrir dans VS Code
Décompressez le ZIP, puis ouvrez le dossier `hautrisque` dans VS Code.

## Voir le site localement
Le site est statique : aucune installation npm ni clé API nécessaire.
Vous pouvez ouvrir `dist/index.html` directement dans un navigateur.
Pour un serveur local, avec Python 3 installé, lancez dans le terminal :

```bash
python3 -m http.server 8000 --directory dist
```

Sous Windows : `py -m http.server 8000 --directory dist`.
Puis ouvrez http://localhost:8000.
Une tâche VS Code « Prévisualiser Haut Risque » est incluse (Python 3 requis).

## Modifier avec Codex
Le fichier `dist/index.html` contient le HTML, les styles CSS dans `<style>` et le JavaScript dans `<script>`.
`dist/assets/` contient toutes les photos, la composition d’accueil et les logos utilisés, ainsi que l’ancien logo conservé dans le projet.
Demandez à Codex de modifier ces fichiers, puis vérifiez le résultat localement.
Les filtres et la galerie en plein écran fonctionnent sans serveur applicatif.

## Publication
Le site public actuel est https://hautrisque.com et reste hébergé par Sites de ChatGPT.
Modifier cette copie locale ne met pas automatiquement le site public à jour.
Le fichier `.openai/hosting.json` conserve la configuration d’origine Sites ; il n’est pas nécessaire pour travailler localement.
Aucun identifiant, jeton de connexion ou historique Git n’est inclus.
Les images sont les versions du site actuel, pas les originaux photo en pleine résolution.
