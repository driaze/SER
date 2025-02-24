# Etude comparative de reconnaissance sonore des émotions (SER)

La reconnaissance sonore des émotions (Speech Emotion Recognition) est un domaine de l’intelligence artificielle qui permet de détecter l’émotion du locuteur à travers la voix. C’est généralement un sous-domaine de la reconnaissance des émotions, jumelé avec la reconnaissance faciale des émotions.

L'objet de cette étude comparative est de comparer les différents algorithmes d'apprentissage automatique (Machine Learning).

## Le dataset ANAD (Arabic Natural Audio Dataset) :

C'est l'un des rares [darasets en arabe](https://github.com/OmarMohammed88/AR-Emotion-Recognition) présents sur le net.

Huit vidéos d'appels en direct entre un présentateur et un auditeur à l'extérieur du studio ont été téléchargées à partir de talk-shows arabes en ligne. Chaque vidéo a ensuite été divisée en tours : appelants et récepteurs. Pour étiqueter chaque vidéo, 18 auditeurs ont été invités à écouter chaque vidéo et à sélectionner s'ils percevaient une émotion heureuse, en colère ou surprise. Le silence, les rires et les morceaux bruyants ont été supprimés. Chaque morceau a ensuite été automatiquement divisé en unités de parole de 1 seconde formant notre corpus final composé de 1384 enregistrements.

Le seul désagrément de ce dataset est l'obfuscation des fichiers .wav, ce qui nou aurait permis d'utiliser les MFCCs pour la génération des features.

Lien de téléchargement : https://www.kaggle.com/datasets/suso172/arabic-natural-audio-dataset/metadata

# Installation 
A : Sur collab :
1. Uploader le fichier ANAD_normalized.csv dans la racine de Google Drive
2. Uploader le fichier le fichier etude_comparative.ipynb dans la racine de google drive
3. Double click sur le fichier etude_comparative.ipynb

B : En local
1. Mettre le fichier etude_comparative.ipynb dans un dossier.
2. Créer un dossier à l'interieur avec le nom "data".
3. Mettre le fichier ANAD_normalized.csv dans le dossier "data"
4. Supprimer les lignes :
from google.colab import drive
drive.mount('/content/drive/')
5. Replacer la ligne : DATA_DIR = '/content/drive/My Drive/'
par : DATA_DIR = 'data/'
