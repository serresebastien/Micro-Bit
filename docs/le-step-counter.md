---
title: 5- Le Step Counter
nav_order: 5
---

# Le Step Counter

## Objectif de la fiche

* Savoir utiliser la fonction « On shake »
* Utiliser des varaibles

## Partie programmation

Commençons par créer la variable « steps » qui recevra notre nombre de pas chaque fois que le Micro-bit sentira un mouvement.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/stepcounter/01.png?raw=true">

Il faut maintenant initialiser notre variable à 0 à la mise sous tension de notre Micro-bit.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/stepcounter/02.png?raw=true">

Afin de détecter le nombre de pas que nous faisons, nous allons utiliser l’accéléromètre de notre carte Micro-bit. Pour se faire, rendez-vous dans la partie « Input » et choisissez le bloc « On shake ».

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/stepcounter/03.png?raw=true">

*À noter que le bloc « change … by … », ne remplace pas notre variable, mais l’incrémente de la valeur passé en paramètre.*

Enfin, nous affichons la variable sur l’écran de notre carte comme ci-dessous.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/stepcounter/04.png?raw=true">

## Partie pratique

Maintenant que notre programme est terminé et téléverser dans notre Micro-bit, il faut trouver un moyen de le fixer sur une jambe de notre pantalon (carte + pile). Armez-vous de scotch et de trombones et allez-y !

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/stepcounter/05.png?raw=true">
<img src="https://github.com/serresebastien/MicroBit/blob/master/img/stepcounter/06.png?raw=true">

## Pour aller plus loin

Proposez maintenant aux enfants de rajouter un petit bout de code nous permettant d’afficher la distance en mètre que nous avons parcouru. Cela se résume en une simple conversion. Cette conversion sera différente de chaque enfant car elle est basée sur la distance moyenne qu’ils parcourent lors d’un pas.