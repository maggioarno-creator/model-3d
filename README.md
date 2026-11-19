# Vidéo → Bitmap (mode Photoshop)

Outil HTML autonome qui convertit une vidéo en vidéo **1-bit** (noir & blanc pur), en temps réel, avec les mêmes paramètres que **Image > Mode > Bitmap…** de Photoshop.

**Fichier : [bitmap.html](bitmap.html)** — à ouvrir directement dans un navigateur, aucun serveur ni installation requis.

## Fenêtre « Bitmap »
- **Résolution** : Entrée (72 px/pouce) et Sortie en pixels/pouce — la vidéo est ré-échantillonnée selon ce ratio.
- **Mode « Avec : »**
  - **50 % Seuil**
  - **Motif géométrique** (matrice de Bayer 8×8)
  - **Diffusion** (Floyd–Steinberg)
  - **Trame de demi-teintes…**

## Fenêtre « Trame de demi-teintes »
- **Linéature** (lignes/pouce) — taille de cellule = sortie ÷ linéature
- **Angle** (degrés)
- **Forme** : Cercle, Losange, Ellipse, Droite, Carré, Croix
- Boutons **Charger… / Enregistrer…** pour les presets (JSON)

## Fonctions vidéo
- Glisser-déposer du fichier (mp4, webm, mov…)
- Aperçu temps réel avec lecture/pause, timeline et boucle
- **Exporter la vidéo (WebM)** — video bitmap avec piste audio, générée dans le navigateur
- **Image PNG** — export de l'image affichée
