# Projet d'Analyse et Prédiction de Survie du Titanic

## Description
Ce projet utilise le célèbre jeu de données du Titanic pour créer un modèle de machine learning capable de prédire la survie des passagers. Le modèle est basé sur une forêt aléatoire (Random Forest) et prend en compte différentes caractéristiques des passagers comme l'âge, le sexe, la classe de voyage, etc.

## Structure du Projet 

```
titanic-prediction/
│
├── data/
│ ├── data.csv # Données d'entraînement
│ └── data_to_predict.csv # Données à prédire
│
├── model/
│ ├── TitanicJupiter_Model.pkl # Modèle entraîné
│ └── columns_fit.pkl # Colonnes utilisées pour l'entraînement
│
├── notebooks/
│ ├── TitanicJupiter_Model.ipynb # Notebook d'entraînement
│ └── TitanicJupyterDataToPredict.ipynb # Notebook de prédiction
│
└── README.md
```


## Fonctionnalités
- Analyse exploratoire des données du Titanic
- Prétraitement des données (gestion des valeurs manquantes, encodage, etc.)
- Entraînement d'un modèle de Random Forest
- Évaluation des performances du modèle
- Prédiction sur de nouvelles données

## Technologies Utilisées
- Python 3.12
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Installation
1. Clonez le repository :

```bash
git clone [URL_DU_REPO
```

2. Installez les dépendances :

```bash
pip install -r requirements.txt
```

## Utilisation
1. **Pour entraîner le modèle** :
   - Ouvrez `notebooks/TitanicJupiter_Model.ipynb` dans Jupyter Notebook
   - Exécutez les cellules dans l'ordre pour :
     - Charger et prétraiter les données
     - Entraîner le modèle
     - Évaluer les performances
     - Sauvegarder le modèle

2. **Pour faire des prédictions** :
   - Placez vos données à prédire dans `data/data_to_predict.csv`
   - Ouvrez `notebooks/TitanicJupyterDataToPredict.ipynb`
   - Exécutez les cellules pour obtenir les prédictions dans `predicted_results.csv`

## Performance du Modèle
Le modèle Random Forest atteint les performances suivantes :
- Précision globale : 81%
- Classe 0 (Non-survivants) :
  - Précision : 79%
  - Rappel : 89%
  - F1-score : 84%
- Classe 1 (Survivants) :
  - Précision : 83%
  - Rappel : 71%
  - F1-score : 76%

## Structure des Données
Les données d'entrée doivent contenir les colonnes suivantes :
| Colonne | Description |
|---------|-------------|
| PassengerId | Identifiant unique du passager |
| Pclass | Classe de la cabine (1, 2, 3) |
| Name | Nom du passager |
| Sex | Genre (male/female) |
| Age | Âge en années |
| SibSp | Nombre de frères/sœurs/époux à bord |
| Parch | Nombre de parents/enfants à bord |
| Ticket | Numéro du ticket |
| Fare | Prix du billet |
| Cabin | Numéro de cabine |
| Embarked | Port d'embarquement (C = Cherbourg, Q = Queenstown, S = Southampton) |

## Auteur
[Votre Nom]

## Licence
Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## Contributions
Les contributions sont les bienvenues ! Pour contribuer :
1. Fork le projet
2. Créer une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push sur la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

## Contact
- Email : [votre-email@example.com]
- LinkedIn : [votre-profil-linkedin]
- GitHub : [@votre-username]

## Remerciements
- Kaggle pour le jeu de données du Titanic
- La communauté open source pour les bibliothèques utilisées
- Tous les contributeurs du projet

Les principales améliorations apportées sont :
1. Meilleure mise en forme de l'arborescence du projet
2. Ajout de commandes bash formatées correctement
3. Ajout d'un tableau pour la structure des données
4. Instructions d'utilisation plus détaillées
5. Meilleure organisation des sections Contact et Contributions
6. Ajout de chemins plus précis pour les notebooks
7. Ajout de descriptions pour les colonnes de données
8. Suggestion de licence MIT par défaut
9. Format plus professionnel pour les informations de contact
