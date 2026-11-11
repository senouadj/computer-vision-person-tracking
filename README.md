# 🎯 Suivi de personnes par vision par ordinateur

Projet final de la formation **Deep Learning & Vision par ordinateur** : détecter des objets (personnes) dans une vidéo, de manière autonome, avec un modèle de détection de type YOLO exécuté sur Google Colab.

## 📌 Objectif

Prendre une vidéo, détecter automatiquement les objets présents image par image, puis produire une vidéo annotée avec des boîtes englobantes. Le projet compare l'effet de plusieurs réglages sur la qualité de la détection.

## 🛠️ Outils utilisés

- Python
- Google Colab (notebook exécutable du début à la fin)
- Modèle de détection YOLO
- OpenCV pour la lecture et l'écriture des vidéos

## 📊 Résultats

Nombre de boîtes détectées selon le seuil de confiance :

| Seuil de confiance | Boîtes détectées |
|--------------------|------------------|
| 0.25               | 1018             |
| 0.50               | 946              |
| 0.70               | 854              |

Un **filtre de taille** (`min_area = 3000`, seuil 0.40) a aussi été testé pour écarter les petites détections parasites : on passe de **976 à 793 boîtes**.

## 📁 Contenu du dépôt

| Fichier | Description |
|---------|-------------|
| `projet de senouadjogan.ipynb` | Notebook commenté (code complet) |
| `istockphoto-1388796730-640_adpp_is.mp4` | Vidéo d'origine |
| `annotée_seuil_050.mp4` | Vidéo annotée avec un seuil de 0.50 |
| `après_filtre.mp4` | Vidéo annotée après filtre de taille |
| `Bilan_Projet_Detection_Video…pdf` | Bilan du projet (erreurs du modèle, limites) |
| `Projet_final_AfriAI.pdf` | Rapport du projet final |

## ▶️ Utilisation

1. Ouvrir le notebook dans Google Colab.
2. Importer la vidéo d'origine dans l'environnement Colab.
3. Exécuter toutes les cellules (**Exécution → Tout exécuter**).
4. Récupérer les vidéos annotées générées.

## 👤 Auteur

**ADJOGAN Senou Gbenoukpo**, étudiant en Système informatique et logiciel, passionné d'IA.
GitHub : (https://github.com/senouadj)
