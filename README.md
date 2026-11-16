# Ajustement de cercles et d'ellipses par moindres carrés

**Optimisation numérique · Moindres carrés · Géométrie · Python / Jupyter**

## Objectif

À partir d'un nuage de points du plan, rechercher le cercle, puis l'ellipse, qui représente le mieux les observations. Ce projet d'optimisation compare différentes formulations d'un problème d'ajustement géométrique et met en évidence le rôle du choix de la fonction objectif et des contraintes.

Le travail s'appuie sur l'article de **Gander, Golub et Strebel (1994)** consacré à l'ajustement de cercles et d'ellipses par moindres carrés.

## Problème mathématique

Pour des points observés \((x_i,y_i)\), un cercle de centre \((a,b)\) et de rayon \(r\) vérifie idéalement :

$$(x_i-a)^2+(y_i-b)^2=r^2.$$

En présence de bruit ou d'erreurs de mesure, on cherche des paramètres qui minimisent un critère d'écart. Plusieurs formulations peuvent être envisagées, notamment :

- **Ajustement algébrique linéarisé** : exploitation d'une reformulation linéaire pour obtenir une estimation initiale.
- **Ajustement géométrique non linéaire** : minimisation des résidus liés aux distances des points au cercle.
- **Ajustement sous contraintes** : prise en compte des conditions nécessaires aux paramètres géométriques.
- **Extension aux ellipses** : élaboraton d'une méthode plus générale permettant d'ajuster des ellipses.

## Contenu du dépôt

```text
notebook_final.ipynb   # Code, calculs et visualisations
projet_cercle.pdf      # Énoncé ou document de référence du projet
data1.txt              # Premier jeu de données
data2.txt              # Second jeu de données
README.md
LICENSE
```

## Référence

Gander, W., Golub, G. H., & Strebel, R. (1994). *Least-squares fitting of circles and ellipses*. BIT, 34, 558–578. https://doi.org/10.1007/BF01934268

**Autrice :** [Nour Bouabid](https://github.com/NourBouabid). **Licence :** MIT (voir `LICENSE`).

