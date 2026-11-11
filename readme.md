# 🏦 Plateforme intelligente de gestion des risques bancaires par le Machine Learning

## 📌 Présentation du projet

Ce projet consiste à développer une plateforme intelligente d'analyse et de gestion des risques bancaires basée sur les techniques de Data Science et de Machine Learning.

L'objectif est d'exploiter plusieurs bases de données financières réelles et publiques afin de construire des modèles prédictifs capables d'identifier, d'évaluer et d'anticiper différents risques bancaires.

La plateforme permettra notamment de :
- Prédire les risques de défaut de remboursement des crédits.
- Détecter les transactions bancaires frauduleuses.
- Estimer les pertes financières potentielles liées aux prêts.
- Segmenter les clients selon leurs comportements financiers.
- Détecter les comportements financiers inhabituels.

Le projet aboutira à une application interactive développée avec **Streamlit**, permettant de visualiser les résultats des modèles et d'explorer les différents modules d'analyse.

---

## 🎯 Objectifs du projet

Les principaux objectifs sont :

- Collecter et exploiter plusieurs datasets financiers réels.
- Réaliser une analyse exploratoire approfondie (EDA).
- Identifier et traiter les valeurs manquantes, aberrantes et dupliquées.
- Analyser et gérer le déséquilibre des classes.
- Développer des modèles de classification pour le scoring de crédit et la détection de fraude.
- Construire des modèles de régression pour estimer les pertes financières.
- Appliquer des algorithmes de clustering pour segmenter les clients.
- Détecter les anomalies dans les comportements financiers.
- Comparer et optimiser les performances des modèles.
- Interpréter les prédictions à l'aide de SHAP.

---

## 🧩 Modules fonctionnels

### 1. Scoring de crédit (Credit Scoring)

**Objectif :** Prédire la probabilité qu'un client rencontre des difficultés de remboursement.

Fonctionnalités :
- Analyse du profil financier du client.
- Calcul d'un score de risque.
- Classification des clients selon leur niveau de risque.
- Identification des facteurs influençant la prédiction.
- Comparaison de plusieurs modèles de classification.

### 2. Détection de fraude (Fraud Detection)

**Objectif :** Identifier les transactions présentant un risque de fraude.

Fonctionnalités :
- Classification des transactions.
- Détection des anomalies.
- Gestion du déséquilibre des classes.
- Optimisation du seuil de décision.
- Analyse des faux positifs et des faux négatifs.

### 3. Prévision financière (Financial Loss Prediction)

**Objectif :** Estimer les pertes financières potentielles associées aux prêts.

Fonctionnalités :
- Prévision du montant des pertes financières.
- Estimation des montants non remboursés.
- Analyse des facteurs influençant les pertes.
- Comparaison de plusieurs modèles de régression.

### 4. Segmentation client (Customer Segmentation)

**Objectif :** Identifier des groupes de clients présentant des comportements financiers similaires.

Fonctionnalités :
- Création de profils clients.
- Regroupement des clients selon leurs comportements financiers.
- Réduction de dimensionnalité.
- Visualisation et interprétation des clusters.

---

## 📊 Sources de données

Le projet repose sur cinq datasets publics provenant de différentes sources.

| Dataset | Source | Utilisation |
|---|---|---|
| Home Credit Default Risk | Kaggle | Scoring de crédit |
| Default of Credit Card Clients | UCI | Comparaison des modèles de crédit |
| Credit Card Fraud Detection | Kaggle | Détection de fraude |
| Lending Club Loan Data | Kaggle | Estimation des pertes financières |
| Bank Marketing | UCI | Segmentation et comportement client |

### Liens de téléchargement

1. **Home Credit Default Risk :**  
   https://www.kaggle.com/competitions/home-credit-default-risk/data

2. **Default of Credit Card Clients :**  
   https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients

3. **Credit Card Fraud Detection :**  
   https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

4. **Lending Club Loan Data :**  
   https://www.kaggle.com/datasets/wordsforthewise/lending-club

5. **Bank Marketing :**  
   https://archive.ics.uci.edu/dataset/222/bank+marketing

---

## 🤖 Algorithmes de Machine Learning

### Classification
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- LightGBM

### Régression
- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

### Clustering
- K-Means
- DBSCAN
- Hierarchical Clustering
- Gaussian Mixture Models (GMM)

### Détection d'anomalies
- Isolation Forest
- Local Outlier Factor (LOF)
- One-Class SVM

### Réduction de dimensionnalité
- PCA
- UMAP

---

## 🔬 Méthodologie

Le projet suit une démarche structurée en plusieurs étapes :

1. **Collecte des données :** récupération des cinq datasets publics.
2. **Analyse exploratoire (EDA) :** étude descriptive, distributions, corrélations et qualité des données.
3. **Nettoyage :** traitement des valeurs manquantes, aberrantes et dupliquées.
4. **Prétraitement :** encodage, normalisation et gestion du déséquilibre des classes.
5. **Feature Engineering :** création et sélection de variables pertinentes.
6. **Modélisation :** entraînement des modèles supervisés et non supervisés.
7. **Évaluation :** comparaison des performances des différents algorithmes.
8. **Optimisation :** amélioration des modèles et réglage des hyperparamètres.
9. **Interprétabilité :** utilisation de SHAP pour comprendre les prédictions.
10. **Déploiement :** développement d'une interface interactive avec Streamlit.

---

## 📈 Évaluation des modèles

Les métriques suivantes seront utilisées :

### Classification
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC
- Confusion Matrix

### Régression
- MAE
- RMSE
- R²

### Clustering
- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index

Le choix des métriques dépendra des objectifs métier et des caractéristiques de chaque dataset.

---

## 🏗️ Architecture du projet

L'architecture globale suit le processus suivant :

```text
Sources de données
       |
       v
Collecte et stockage
       |
       v
Nettoyage et préparation
       |
       v
Analyse exploratoire (EDA)
       |
       v
Feature Engineering
       |
       v
Modules de Machine Learning
       |
       +----------------------+
       |          |           |
       v          v           v
  Credit      Fraud       Financial
  Scoring   Detection       Loss
       |          |           |
       +----------+-----------+
                  |
                  v
          Customer Segmentation
                  |
                  v
       Évaluation et interprétation
                  |
                  v
          Application Streamlit
                  |
                  v
         Rapports et recommandations
```

---

## 📁 Structure du projet

La structure proposée pour le dépôt est la suivante :

```text
banking-risk-ml-platform/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
│
├── notebooks/
│   ├── 01_home_credit_eda.ipynb
│   ├── 02_credit_card_eda.ipynb
│   ├── 03_fraud_detection_eda.ipynb
│   ├── 04_lending_club_eda.ipynb
│   └── 05_bank_marketing_eda.ipynb
│
├── src/
│   ├── data/
│   │   ├── load_data.py
│   │   └── preprocessing.py
│   │
│   ├── features/
│   │   └── feature_engineering.py
│   │
│   ├── models/
│   │   ├── credit_scoring.py
│   │   ├── fraud_detection.py
│   │   ├── financial_prediction.py
│   │   └── customer_segmentation.py
│   │
│   └── evaluation/
│       └── metrics.py
│
├── models/
│   ├── credit_scoring/
│   ├── fraud_detection/
│   ├── financial_prediction/
│   └── customer_segmentation/
│
├── app/
│   ├── Home.py
│   ├── pages/
│   │   ├── 01_Credit_Scoring.py
│   │   ├── 02_Fraud_Detection.py
│   │   ├── 03_Financial_Prediction.py
│   │   └── 04_Customer_Segmentation.py
│   └── utils/
│
├── reports/
│   ├── figures/
│   └── results/
│
├── requirements.txt
├── .gitignore
└── README.md
```


---

## 🚀 Installation et exécution

### 1. Cloner le dépôt

```bash
git clone https://github.com/BayeGallasse-1719/Bank-risk-Ml.git
cd banking-risk-ml-platform
```

### 2. Créer un environnement virtuel

```bash
python -m venv venv
```

Activation sous Windows :

```bash
venv\Scripts\activate
```

Activation sous Linux / macOS :

```bash
source venv/bin/activate
```

### 3. Installer les dépendances

```bash
pip install -r requirements.txt
```

### 4. Ajouter les datasets

Télécharger les cinq bases de données depuis les sources indiquées précédemment et les placer dans les dossiers appropriés de `data/`.

### 5. Lancer l'application Streamlit

```bash
streamlit run app/main.py
```

---

## 📦 Livrables attendus

Le projet devra aboutir aux livrables suivants :

1. Rapport de cadrage et de compréhension des données.
2. Notebook d'analyse exploratoire pour chaque dataset prioritaire.
3. Notebooks de préparation et de Feature Engineering.
4. Modèles de classification entraînés et évalués.
5. Modèles de régression entraînés et évalués.
6. Modèles de clustering et de détection d'anomalies.
7. Rapport comparatif des performances.
8. Pipelines reproductibles de Machine Learning.
9. Application interactive développée avec Streamlit.
10. Rapport final présentant les résultats, les limites et les recommandations.

---

## ⚠️ Limites et considérations éthiques

Les datasets utilisés sont publics et proviennent de contextes différents.

Les modèles développés constituent des prototypes pédagogiques et ne doivent pas être utilisés directement pour prendre des décisions bancaires réelles.

Une attention particulière sera accordée :
- Aux biais algorithmiques.
- À la protection des données personnelles.
- À l'explicabilité des décisions.
- Aux faux positifs et faux négatifs.
- À la représentativité des données.
- Aux limites de généralisation des modèles.

---

## 🏁 Résultat final attendu

Une plateforme pédagogique intelligente de gestion des risques bancaires permettant d'explorer plusieurs problématiques financières grâce à des techniques de Machine Learning intermédiaires et avancées.

L'application permettra de centraliser les résultats des différents modèles, de visualiser les prédictions et de fournir des éléments d'aide à l'analyse des risques bancaires.

---

## 👨‍💻 Auteur: BayeGallasse

Projet Data Science & Machine Learning.

**Domaine :** Banque, Finance et Intelligence Artificielle.

**Technologies principales :** Python, Scikit-learn, XGBoost, LightGBM, SHAP et Streamlit.