---
title: 4- La boussole
nav_order: 4
---

# La boussole

## Objectif de la fiche

* Utiliser le bloc « Compass »
* Savoir utiliser les conditions

## Première partie

Pour coder notre compas, commençons avec le bloc « forever » dans lequel nous allons initialiser une variable (ici degrees) à l’aide du capteur « compass » de notre Micro-bit, comme ci-dessous :

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/boussole/01.png?raw=true">

À noter que le bloc « compass heading » utiliser se trouve dans la partie « Input » de notre menu.

Utilisons maintenant le bloc de condition « if » pour déterminer vers quelle direction nous orientons notre carte. A l’aide de l’image de boussole ci-dessous nous pouvons facilement attribuer chaque point cardinal à une plage précise en degrés :

* Nord de 315 à 45 degrés
* Est de 45 à 135 degrés
* Sud de 135 à 225 degrés
* Ouest de 225 à 315 degrés

<img style="with:200px" src="https://github.com/serresebastien/MicroBit/blob/master/img/boussole/02.png?raw=true">

Une fois avoir fait réfléchir les enfants les points cardinaux, voici le code nécessaire afin d’indiquer le bon point cardinal en fonction de l’orientation en degrés de notre Micro-bit.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/boussole/03.png?raw=true">