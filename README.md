# Projet de Modélisation et Machine Learning - Diagramme de Hertzsprung-Russell (HR)

**Auteurs : Monija SIVARAJAH - Sara E. VELASCO CALDERON**

## Introduction

Ce projet explore l'application de machine learning pour l'analyse du diagramme de Hertzsprung-Russell (HR). Le diagramme HR est un outil fondamental en astrophysique, permettant de représenter la magnitude absolue des étoiles en fonction de leur indice de couleur (B-V). Cette représentation graphique est essentielle pour distinguer et classifier différentes populations stellaires, telles que la séquence principale, les géantes, les supergéantes et les naines blanches.


## Objectif 

L'objectif principal de ce projet est d'utiliser des méthodes d'apprentissage non supervisé pour identifier et caractériser les types d'étoiles au sein du diagramme HR.



## Données

Le dataset utilisé est issu du **catalogue Hipparcos**, disponible sur Kaggle : [Hipparcos Star Catalog](https://www.kaggle.com/datasets/konivat/hipparcos-star-catalog/data)

## Méthodologie


  * **Prétraitement des données** 
  * **Réduction de dimension (PCA)** 
  * **Apprentissage non supervisé (clustering : K-Means, DBSCAN, GMM)** 
  * **Évaluation du modèle pour le clustering**
  * **Labellisation des données**
  * **Apprentissage supervisé (classification : Random Forest)**
  * **Évaluation du modèle pour la classification (matrice de confusion, accuracy, precision, recall, f1-score...)**


## Résultats 

Le modèle a permis de distinguer les principaux types stellaires. Cependant, un fort déséquilibre des classes a été observé, affectant particulièrement la détection des catégories rares comme les naines blanches (faible rappel).


## Pistes d'amélioration

* Utiliser un jeu de données plus riche en informations sur les naines blanches, ou supposer l'existence de seulement trois groupes distincts.
* Déterminer à l’avance le nombre optimal de composantes principales pour la PCA en traçant la courbe de la variance expliquée cumulée en fonction du nombre de composantes.
* Ajuster les paramètres de l’algorithme DBSCAN pour améliorer la qualité du clustering.
* Réduire le nombre de variables utilisées lors de l'application de la PCA afin de se concentrer sur les caractéristiques les plus pertinentes.

## Licence 
Ce projet est sous licence MIT. Consultez le fichier [LICENSE](./LICENSE)pour plus de détails sur les conditions de licence.

