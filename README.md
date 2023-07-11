# Feature_engineering_and_optimization_model_hyper_parameters_EDA_to_ML
Améliorer les performances de 10 modèles de ML via du Feature engineering, optimization model hyper-parameters with GridSearchCV &amp; applying techniques like boosting, stacking and voting



## Objectif

L’objectif principal de ce use case est d’améliorer les performances de 10 modèles de ML en :

- utilisant des features construites à partir des features existantes (Feature Engineering)

- optimisant les hyperparamètres du modèle avec GridSearchCV

- appliquant des techniques telles que le boosting, l'empilage et le vote




## Démarche 

J’ai scindé ce use case en 2 notebooks.

Cf. les 2 notebooks ci-joints.

Ces notebooks explorent l'utilisation de base de Pandas et scikit-learn pour un problème de classification.

Le second notebook aborde des approches plus avancées comme l'utilisation des graphiques Seaborn, le Feature Engineering, GridSearch CV et les modèles ML basés sur l'empilement et le vote




## 1er notebook : EDA, Data wrangling, Scikit-learn ML algorithms & Comparison of Model results

Le 1er notebook porte sur :
- une analyse exploratoire des données du dataset selectionné,
- un traitement des données, à savoir remplir les nan, convertir les données catégorielles en données numériques, créer des données d'entraînement et de test pour les algorithmes de ML

- l’implémentation de plusieurs algorithmes de ML Scikit-learn : implémenter différents classificateurs de la bibliothèque sklearn (Régression logistique, Bayes naïf gaussien, KNN, Arbre de décision, Forêt aléatoire, SVM)
- la comparaison des résultats de ces modèles en utilisant des métriques comme confusion_matrix, classification_report, accuracy_score et implémenter la validation croisée k fold pour la comparaison des résultats des tests




## 2ème notebook : Feature engineering, optimization model hyper-parameters with GridSearchCV & applying techniques like boosting, stacking and voting

Le 2ème notebook porte sur 
- une analyse exploratoire des données du dataset selectionné, mais en utilisant cette fois-ci seaborn :
    . Cartes thermiques Seaborn : données manquantes dans df_train et df_test
    . Diagrammes de comptage de Seaborn : Nombre de (non-)survivants en fonction des caractéristiques
    . Diagrammes de distribution de Seaborn : Distribution de l'âge et du poids en fonction de la classe de probabilité, du sexe et du nombre de survivants
    . Diagrammes à barres et diagrammes en boîte pour les caractéristiques catégorielles : Pclass et Embarqué
    . Diagrammes de violon et d'essaim de Seaborn : Survivants en fonction de l'âge, de la classe de P et du sexe


- le traitement des données et Feature Engineering à savoir :

    . Feature Engineering : inclure de nouvelles caractéristiques pour améliorer les performances des classificateurs et combler les valeurs manquantes :
    Taille de la famille, Personne seule, Longueur du nom, Titre

    . Data Wrangling : remplir les valeurs NaN, convertir les valeurs catégorielles en valeurs numériques, échelle standard, créer X, y et X_test pour la dernière partie de ce notebook (ci-dessous)


- l’optimisation des paramètres du classificateur, Boosting, Voting et Stacking :

    . Révision : validation croisée k fold pour SVC et Random Forest :
    SVC, caractéristiques non mises à l'échelle
    SVC, caractéristiques mises à l'échelle
    Random Forest Classifier, RFC, caractéristiques non mises à l'échelle

    . Réglage des hyperparamètres avec GridSearchCV et RandomizedSearchCV pour :
    Classificateur de machine à vecteur de support, SVC
    K Plus Proche Voisin, KNN
    Arbre de décision
    Classificateur Random Forest, RFC

    . étudier les modèles d'ensemble tels que Boosting, Stacking et Voting :
    ExtraTreesClassifier
    Gradient Boost Decision Tree - GBDT (arbre décisionnel à gradient de croissance)
    eXtreme Gradient Boosting - XGBoost
    Adaptive Boosting - AdaBoost
    CatBoost
    Voting : VotingClassifier 1, VotingClassifier 2
    Empilage : StackingClassifier

    . Comparer les performances d'un classificateur sur la base du score de validation : graphique de comparaison

    . Corrélation des résultats de prédiction : matrice de corrélation

















