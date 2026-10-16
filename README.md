# Prédiction du diabète par Machine Learning

Projet de groupe réalisé à l'Institut Supérieur d'Informatique (ISI), année académique 2025-2026.

## Description
Construction et comparaison de deux modèles de classification capables de prédire si une personne est susceptible d'être diabétique à partir de huit caractéristiques médicales. Travail réalisé en Python avec Google Colab.

## Données
768 observations, 8 variables explicatives (grossesses, glucose, pression artérielle, épaisseur de peau, insuline, IMC, antécédents familiaux, âge) et une variable cible `Outcome` (0 = non diabétique : 500 cas, 1 = diabétique : 268 cas).

## Méthode
1. Exploration des données (dimensions, valeurs manquantes, statistiques, répartition de la cible)
2. Séparation entraînement / test : 80 % / 20 % (stratifiée)
3. Standardisation (`StandardScaler`, ajusté uniquement sur l'entraînement)
4. Modèle 1 : Régression logistique
5. Modèle 2 : Random Forest (100 arbres)
6. Évaluation : accuracy, matrice de confusion, rapport de classification, importance des variables

## Résultats
| Modèle | Accuracy | F1 (classe diabétique) | Faux négatifs |
|---|---|---|---|
| Régression logistique | 71,43 % | 0,56 | 26 |
| Random Forest | 75,97 % | 0,63 | 22 |

Le glucose est la variable la plus importante, suivie de l'IMC, de l'âge et des antécédents familiaux.

## Limites
Environ un quart des cas diabétiques reste mal détecté. Ce projet est un exercice pédagogique et **non un outil de diagnostic médical**.

## Technologies
Python, pandas, scikit-learn, matplotlib, Google Colab

## Contenu du dépôt
- `docs/machinelearning.pdf` : rapport complet
- `notebook.ipynb` : à ajouter (export du notebook Colab : Fichier > Télécharger > .ipynb)

## Auteurs
Bintou LO, Badiayeu Saboudou SEYDI, Ndeye Marieme DIALLO, Mahecor DIOUF

Encadrant : M. BARRO
