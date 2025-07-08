# 🧠 Parkinson Off Score Predictor

## 🎯 Objectif du projet

Ce projet a pour but de développer un modèle de prédiction du **score moteur OFF “vrai”** chez les patients atteints de la maladie de Parkinson. Ce score reflète l’état moteur sans l’effet des médicaments dopaminergiques et permet de suivre la progression réelle de la maladie.

---

## 🧾 Contexte

La maladie de Parkinson est un trouble neurodégénératif majeur. L’évaluation du score OFF est souvent imprécise ou absente dans les suivis médicaux. Ce projet vise à prédire ce score à partir d’informations cliniques, démographiques et pharmacologiques disponibles lors des visites patients.

---

## 📁 Structure du projet

```bash
parkinson_offscore_predictor/
├── data/
│   ├── raw/             # Données brutes (X_train, y_train, X_test)
│   └── processed/       # Données nettoyées et enrichies
│
├── scripts/
│   ├── 01_data_cleaning.R         # Nettoyage des données
│   ├── 02_feature_engineering.R  # Transformation et création de variables
│   ├── 03_modeling.R             # Modélisation prédictive
│   └── 04_evaluation.R           # Évaluation des performances
│
├── outputs/
│   ├── predictions/     # Prédictions sur les données de test
│   ├── models/          # Modèles sauvegardés
│   └── figures/         # Visualisations
│
├── report/
│   └── final_report.Rmd # Rapport de projet
│
└── README.Rmd           # Présentation complète du projet
```

---

## 💡 Comment utiliser le projet

### 1. 📦 Installer les packages nécessaires

```r
install.packages(c("tidyverse", "randomForest", "xgboost", "caret", "lubridate", "ggplot2", "naniar", "skimr"))
```

### 2. 📁 Télécharger le projet

Clone ou télécharge ce projet GitHub (ou dézippe le dossier) dans ton environnement local.

### 3. 🔁 Exécuter les scripts dans l’ordre

```r
source("scripts/01_data_cleaning.R")
source("scripts/02_feature_engineering.R")
source("scripts/03_modeling.R")
source("scripts/04_evaluation.R")
```

### 4. 📄 Générer le rapport final

Ouvrir `report/final_report.Rmd` et cliquer sur **"Knit"** dans RStudio.

---

## 📋 Données disponibles

Variables clés : âge, sexe, ledd, temps depuis la prise de médicament, scores ON/OFF, gène, etc.  
Cible : score OFF “vrai”.

---

## 📦 Packages utilisés

- tidyverse
- randomForest / xgboost
- caret / tidymodels
- naniar, skimr
- ggplot2, patchwork

---

## 👨‍💻 Auteur

**Oumar Abdramane ALLAWAN**  

