
# Analyse d’un article scientifique : PASS-CCTV (2024)

##  Référence
**Titre :** PASS-CCTV: Proactive Anomaly Surveillance System for CCTV Footage Analysis in Adverse Environmental Conditions  
**Auteurs :** Hobeom Jeon, Hyungmin Kim, Dohyung Kim, Jeahong Kim  
**Publié dans :** Expert Systems With Applications, Volume 254, 2024

---

##  Problématique

Les systèmes de vidéosurveillance intelligente sont confrontés à trois principaux défis :

1. **Localisation imprécise des piétons** dans des conditions difficiles (brouillard, neige, nuit), ce qui compromet la détection des anomalies.
2. **Détection mono-événement** : la plupart des approches actuelles ne détectent qu’un type d’anomalie à la fois.
3. **Adaptabilité limitée** : la nécessité de réentraîner les modèles pour chaque nouvel environnement augmente les coûts.

---

## Approche proposée

Le système PASS-CCTV se compose de deux modules majeurs :

### 1. Module de détection et suivi humain
- **Méthode de couplage de caractéristiques** : fusion des caractéristiques d'apparence humaine et de détection d'objet.
- **Filtrage des faux positifs** : basé sur l'analyse de la surface parcourue par les trajectoires, plutôt que sur la distance brute.

### 2. Module de reconnaissance interactive des anomalies
- **Détecteur d'intersection** : pour détecter les intrusions et l’errance.
- **Suivi des bagages** : approche top-down sans utilisation du foreground.
- **Détection d’arson** : par analyse sémantique des images à l’aide de prompts texte avec le modèle CLIP.

---

## Technologies utilisées

- Deep Learning (DL)
- Vision par ordinateur (MOT, re-ID, RoI pooling)
- **CLIP (Contrastive Language–Image Pretraining)** pour l’analyse image–texte.
- Calcul de surface polygonale pour la filtration des faux positifs humains.
- Approche **Top-down** pour objets abandonnés.
- RTSP pour les flux vidéo en temps réel.

---

##  Perspectives de recherche

- **Personnalisation via prompts utilisateur** sans besoin de réentraîner les modèles.
- **Réduction des coûts de maintenance** par une meilleure adaptabilité.
- **Extension possible** à d’autres anomalies (violence, vol, etc.) par ajout de nouveaux prompts.
- **Utilisation commerciale** envisageable grâce à sa robustesse en environnement réel.

---

