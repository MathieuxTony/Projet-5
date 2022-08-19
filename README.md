
# Catégoriser automatiquement des questions

Il s'agit de tester différentes méthodes de classification de texte. Les textes considérés
sont des questions posées sur Stack Overflow et l'idée du projet est donc de suggérer des tags
à la personne qui pose une question afin de la classer.  

## Etape 1: préprocessing des données textuelles  

Les données ont été récupérées sur le site Stack Overflow à l'aide de l'outil d'export de données
'StackExchangeDataExplorer'.
Ces données nécessitent un préprocessing important (gestion de la casse, de la ponctuation,
 des balises html...). Le notebook d'exploration présente ce préprocessing.

 ## Etape 2: classification

 On mettra en oeuvre dans le notebook de tests différentes méthodes de classification. On 
 commencera par une approche non supervisée à l'aide de l'algorithme LDA de la bibliothèque Gensim,
 Puis on testera des classifications supervisées sans, et avec, sentence embedding (Word2Vec, 
 BERT et USE).

 ## Etape 3: déploiement de l'application

 On déploiera l'un des modèles à l'aide de streamlit.

