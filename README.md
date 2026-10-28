# CIC-IDS2017 — Détection d’intrusions réseau

## Présentation

Ce projet vise à développer et à comparer des modèles de machine learning pour détecter les intrusions réseau à partir du dataset CIC-IDS2017.

L’objectif est d’étudier les données de trafic réseau, de préparer les caractéristiques, puis d’évaluer différentes approches de détection.

## Structure du projet

```text
projet_data/
├── data/
│   ├── raw/           # Données originales (non versionnées)
│   └── processed/     # Données traitées (non versionnées)
├── models/            # Modèles entraînés
├── notebooks/         # Analyses et expérimentations
├── reports/           # Rapports et résultats
├── scripts/           # Scripts Python
├── nom_du_projet/     # Modules Python du projet
├── .gitignore
├── environment.yml
├── requirements.txt
└── README.md
```

## Travail réalisé

- Inspection des huit fichiers Parquet.
- Vérification des dimensions et des colonnes.
- Traitement des valeurs infinies et manquantes.
- Correction de certains labels mal encodés.
- Fusion des données dans un dataset commun.
- Analyse de la distribution des 15 classes.
- Étude des doublons exacts et des lignes présentant les mêmes caractéristiques avec des labels différents.
- Préparation des caractéristiques et de la cible.
- Préparation d’une séparation entraînement/test en tenant compte des vecteurs de caractéristiques identiques.

## Travail à venir

- Entraîner et évaluer un modèle Random Forest.
- Étudier la détection d’anomalies avec Isolation Forest.
- Explorer un autoencodeur et éventuellement un VAE.
- Interpréter les prédictions avec SHAP.
- Comparer les performances des différentes approches.

## Données

Les fichiers de données CIC-IDS2017 ne sont pas inclus dans ce dépôt GitHub, car ils sont volumineux. Ils doivent être obtenus séparément et placés dans les dossiers locaux prévus par le projet.

Les dossiers `data/raw/` et `data/processed/`, ainsi que les fichiers Parquet, sont exclus du suivi Git.

## Installation

Créer et activer un environnement Python adapté au projet, puis installer les dépendances :

```bash
pip install -r requirements.txt
```

Les notebooks peuvent ensuite être ouverts avec Jupyter Notebook ou JupyterLab.

## Collaboration

Ce dépôt sert à partager les notebooks, les scripts, la documentation et les futurs résultats du projet. Les données brutes et traitées restent locales.
