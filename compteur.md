---
title: 2- Le compteur
nav_order: 2
---

# Notre compteur Micro-bit

## Objectif de la fiche

* Introduction au principe de variable
* Savoir utiliser les boutons A et B de la carte
* Introduction au principe de condition

## Fonction principale incrémentation/décrémentation

Le programme que nous allons réaliser consiste en la réalisation basique d’un compteur. Selon la rapidité de chaque enfant, nous pourrons aller plus ou moins loin avec eux en complexifiant notre programme.

Il va de soi que le but des exercices de programmation n’est pas de donner le code tout fait à l’enfant mais de le mettre sur la piste pour qu’il se mette à chercher par lui-même.

Commençons par créer puis initialiser notre variable « compte » à 0.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/01.png?raw=true">

Or, si vous regardez la simulation où essayer de téléverser le programme dans la carte rien ne s’affichera. Mais pourquoi donc !? Et bien tout simplement car nous ne demandons à aucun moment à notre programme d’afficher notre variable « compte ». Pour se faire, rien de plus simple :

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/02.png?raw=true">

Il faut maintenant pouvoir incrémenter (ajouter 1) et décrémenter (soustraire 1) notre compteur lorsque les boutons A ou B sont pressés.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/03.png?raw=true">

## Fonctionnalités supplémentaires

Le compteur est d’ores et déjà fonctionnel, mais nous pouvons lui ajouter des fonctionnalités comme celle de se remettre à zéro lorsque les deux boutons A et B sont pressés simultanément.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/04.png?raw=true">

Actuellement, notre programme permet à notre compteur d’aller dans les négatifs. Demandez aux enfants de réfléchir sur la façon dont ils pourraient changer cela. Il sera nécessaire de faire intervenir un nouveau bloc : la condition (Si… Alors…).

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/05.png?raw=true">
*La couleur des blocs ci-dessus est différente car ils ne sont pas imbriqués dans une boucle « toujours » ou « au démarrage »*

Une fois la condition trouvée, il faut qu’elle soit vérifiée à tout moment lors que notre programme tourne sur notre carte. Il suffit donc de la placer dans la boucle « toujours » comme ceci :

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/06.png?raw=true">

## Conversion de notre compteur en minuteur

Essayons maintenant de convertir notre en minuteur afin que ce dernier donne le compte à rebours. Nous aimerions qu’un décompte se fasse depuis un nombre en seconde donné en paramètre jusqu’à zéro. Nous avons besoin d’initialiser notre variable « compte » à la valeur en seconde où notre minuteur commencera.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/07.png?raw=true">

Il faut maintenant créer la condition « Si la variable compte est supérieur à 0 alors », décrémenter la variable toutes les 1 secondes. Une fois la variable compte arriver à 0, on la remet à 35 pour réinitialiser notre compteur.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/compteur/08.png?raw=true">
