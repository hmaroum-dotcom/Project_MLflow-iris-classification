# Project_MLflow-iris-classification
# MLflow Iris Classification

Ce projet est une introduction pratique au MLOps avec **MLflow** et **Scikit-Learn**. Il entraîne un modèle Random Forest sur le jeu de données Iris, suit les métriques de performance et enregistre les artefacts (graphiques et modèles).

## 🚀 Fonctionnalités
- Enregistrement automatique et manuel des hyperparamètres.
- Suivi de la métrique de performance (`accuracy`).
- Sauvegarde du graphique des prédictions en tant qu'artefact.
- Versionnage du modèle entraîné avec MLflow Models.

## 🛠️ Installation

1. **Cloner le dépôt :**
   ```bash
   git clone https://github.com
   cd mlflow-iris-classification
   ```

2. **Créer un environnement virtuel (optionnel mais recommandé) :**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Mac/Linux
   # ou
   .\venv\Scripts\activate     # Sur Windows
   ```

3. **Installer les dépendances :**
   ```bash
   pip install -r requirements.txt
   ```

## 📊 Utilisation

1. **Lancer l'entraînement du modèle :**
   ```bash
   python train.py
   ```
   Ce script va générer localement un dossier `mlruns/` contenant toutes les données de l'expérience.

2. **Visualiser les résultats dans l'interface MLflow :**
   ```bash
   mlflow ui
   ```

3. **Accéder à l'application :**
   Ouvrez votre navigateur et rendez-vous sur [http://127.0.0.1:5000](http://127.0.0.1:5000). Vous y trouverez vos paramètres, votre score d'accuracy et le graphique `iris_predictions.png`.

## 📦 Structure du projet
- `train.py` : Script principal d'entraînement et de tracking MLflow.
- `requirements.txt` : Liste des bibliothèques Python requises.
- `.gitignore` : Permet d'éviter d'envoyer le dossier local `mlruns/` sur GitHub.
