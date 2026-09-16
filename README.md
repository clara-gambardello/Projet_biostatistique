# Projet Biostatistique : Cancer du poumon

Projet de biostatistique - Étude cas-témoins sur les facteurs de risque associés au cancer bronchique primitif.

## Le projet

Étude portant sur un jeu de données de 550 individus (230 cas, 320 témoins) recrutés dans les mêmes établissements de soins, visant à établir des liens entre le risque de cancer du poumon et différents facteurs :

* Tabagisme (ancien fumeur, fumeur actuel, jamais)
* Exposition professionnelle et domestique à la fumée
* Bronchopneumopathie chronique
* Âge, sexe, IMC, niveau d'études, région de résidence

## Méthodes statistiques

* **Statistiques descriptives** : boxplots et diagrammes en barres comparant cas et témoins sur l'ensemble des variables
* **Régression logistique** : modèles univariés puis multivariés (sélection par AIC, méthode backward) pour quantifier l'association entre chaque facteur et le risque de cancer
* **Régression polytomique ordonnée** : modélisation des variables ordinales (tabagisme, exposition professionnelle) en fonction du statut cas/témoin et des autres covariables

Tous les intervalles de confiance et conclusions statistiques sont établis avec un niveau de confiance de 95%.

## Résultats principaux

Le tabagisme, l'âge, l'exposition professionnelle à la fumée et la bronchopneumopathie chronique apparaissent comme des facteurs de risque significatifs, tandis qu'un IMC plus élevé et un niveau d'études supérieur semblent avoir un effet protecteur.

## Structure du projet

* `CancerPoumongood.csv` : jeu de données
* `Code_Projet_Biostat.Rmd` : script R Markdown avec l'ensemble des analyses
* `Rapport_Projet_Biostat.pdf` : rapport complet du projet en PDF
* `Description.doc` : description du jeu de données

## Lancer l'analyse

1. Cloner le projet ou télécharger les fichiers
2. Installer les packages nécessaires

```r
install.packages(c("ggplot2", "dplyr", "stringr", "MASS", "esquisse", "patchwork"))
```

3. Ouvrir `Code_Projet_Biostat.Rmd` dans RStudio et compiler (Knit)

## Auteurs

Clara GAMBARDELLO | Karla PEM
Projet de Biostatistiques (2026)
