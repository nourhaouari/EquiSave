# EquiSave
# EquiSave

**EquiSave** est une plateforme web intelligente conçue pour assurer la gestion et la maintenance des équipements médicaux au sein des établissements de santé. Grâce à une interface fluide, des statistiques visuelles et un système de prédiction basé sur l’IA, EquiSave permet aux équipes médicales et techniques de mieux suivre l’état des dispositifs critiques.

## Objectifs du projet

- Centraliser les informations sur les équipements médicaux.
- Suivre l’inventaire de produits et accessoires.
- Permettre aux utilisateurs de soumettre des signalements ou des remarques.
- Générer des prédictions automatiques sur l’état de fonctionnement des équipements grâce à un modèle d’intelligence artificielle.
- Optimiser la prise de décision concernant la maintenance.

## Technologies utilisées

- **Frontend :** HTML, CSS (TailwindCSS), JavaScript
- **Backend :** PHP (avec XAMPP)
- **Base de données :** MySQL
- **IA :** Python (Scikit-Learn, MLPClassifier)
- **API IA :** Flask
- **Versioning :** Git & GitHub

## Fonctionnalités principales

- Authentification : Enregistrement et connexion des utilisateurs.
- Dashboard : Vue globale des équipements, utilisateurs et état de maintenance.
- Équipements : Ajout, consultation et suivi de l’état de chaque appareil.
- Inventaire : Liste complète des produits avec détails techniques.
- Soumissions : Interface pour recevoir les retours ou alertes utilisateurs.
- Historique : Journal des interventions de maintenance.
- Prédiction : Détection automatique du statut des équipements (opérationnel, maintenance, etc.) via un modèle MLP.

## Structure du projet

equisave/
├── app.py # API Flask pour les prédictions
├── models/ # Modèle et scaler entraînés (.pkl)
├── dataset_machines.csv # Données utilisées pour l'entraînement IA
├── dashboard.php
├── equipment.php
├── inventory.php
├── submissions.php
├── historique_maintenance.php
├── login.php / register.php / logout.php
├── db.php # Connexion à la base de données
├── 
└── ...

## Lancement local

1. **Backend :**
   - Assurez-vous d’avoir **XAMPP** installé.
   - Placez le dossier dans `htdocs/`.
   - Lancez **Apache** et **MySQL** via le panneau de XAMPP.
   - Créez une base de données `equisave_db` et importez le fichier SQL fourni (si applicable).

2. **Frontend :**
   - Accédez à `http://localhost/equisave/login.php` via votre navigateur.

3. **API IA :**
   - Lancez le fichier `app.py` dans un environnement Python :
     ```
     python app.py
     ```

## Exemple de prédiction IA

Lorsqu’un nouvel appareil est ajouté, l’IA utilise 12 caractéristiques techniques (heures d'utilisation, température, erreurs, etc.) pour prédire automatiquement son statut : opérationnel, à surveiller, critique ou à entretenir.

## À propos

Ce projet a été réalisé dans le cadre d’un module académique avec pour objectif de combiner développement web et intelligence artificielle pour une application concrète en milieu médical.

## Auteur

Développé par Nour Haouari Rania Guesmi et Nourhene Bellazreg – Étudiantes en Cycle Ingenieur en genie biomedical TTIS

