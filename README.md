# Systèmes de recommandation — M2

Travaux pratiques du module Systèmes de Recommandation (M2), basés sur le dataset
[MovieLens ml-latest-small](https://grouplens.org/datasets/movielens/) (GroupLens Research).

## 📁 Structure du projet

```
├── data/      # dataset (non versionné, voir installation ci-dessous)
│    
├── notebooks/
│   ├── analyse_movielens.ipynb        # TP1 : analyse exploratoire (EDA)
│   └── recommandation_surprise.ipynb  # TP2 : modèles avec la librairie Surprise
├── requirements.txt
└── README.md
```

## ⚙️ Installation

1. Cloner le dépôt puis créer un environnement virtuel :
   ```bash
   python -m venv venv
   venv\Scripts\Activate.ps1      # Windows PowerShell
   # source venv/bin/activate     # Mac/Linux
   ```

2. Installer les dépendances :
   ```bash
   pip install -r requirements.txt
   ```

3. Télécharger le dataset [ml-latest-small.zip](https://grouplens.org/datasets/movielens/)
   et le dézipper dans `data/`, de façon à obtenir `data/movies.csv`, etc.

## 📓 Contenu

- **TP1 — Analyse exploratoire** : chargement des données, matrice utilisateurs × films,
  statistiques sur les notes, films/genres les plus populaires et les mieux notés.
- **TP2 — Librairie Surprise** : construction du dataset, système de recommandation
  aléatoire (`NormalPredictor`) et système baseline (`BaselineOnly`), évalués en MAE/RMSE.

## Auteur

Mohcine ERGUI — M2, module Systèmes de Recommandation
