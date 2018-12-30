---
title: 9- Le jeu du météor
nav_order: 9
---

# Le jeu du météor

## Objectif de la fiche

* Réaliser son premier jeu entièrement sur Micro-bit
* Savoir utiliser les blocs `plot` et `unplot`
* Se repérer dans un repère cartésien XY

## Première étape, faire bouger le LED du joueur

Nous allons utiliser les boutons A et B pour aller à gauche et à droite. Pour garder une trace de l'emplacement de l'utilisateur, nous devons utiliser une variable qui stockera la position X de notre joueur.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/01.png?raw=true">

Maintenant, demandez aux enfants de faire en sorte de pouvoir déplacer le joueur à l’aide des bloc `plot` et `unplot`.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/02.png?raw=true">

Téléverser le code sur la carte Micro-bit. Que se passe-t-il lorsque vous cliquez sur A lorsque le voyant est complètement à gauche ? Laissez les enfants essayer leur code et donnez-leur des pistes afin de corriger les mouvements du joueur.

## Deuxième étape, corrigeons les déplacements du joueur

La LED représentant le joueur sort de notre écran quand nous allons trop loin sur les côtés.

Afin de corriger cela, il faut forcer notre variable `player` à rester entre 0 et 4 strictement.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/03.png?raw=true">

Nous souhaitons également commencer avec notre joueur au milieu de l’écran. Nous pouvons le faire en appuyant sur les deux boutons A+B en même temps qui vont réinitialiser la position et redémarrer le jeu.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/04.png?raw=true">

Téléverser le code dans notre carte et faite encore tester les enfants. Si tout a bien été réalisé le joueur reste maintenant visible sur notre écran et ne disparaît plus.

## Troisième étape, les météores

Maintenant que notre joueur peut se déplacer, attaquons-nous aux météores.

Ces derniers commencent à une position aléatoire sur la rangée supérieure de l’écran et tombent progressivement vers le bas. Nous avons donc besoin de deux variables pour contrôler la position des météores selon X et Y, `meteor-x` et `meteor-y`.

`meteor-x` est mis à une valeur aléatoire entre 0 et 4, et `meteor-y` est contrôlé par une boucle for qui met le météore y de 0 à 4 toutes les 100ms.

Le code pour les météores doit se mettre dans l’évènement `A+B pressés`.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/05.png?raw=true">

Quand le météore atteint la rangée du bas, nous devons voir si le météore a frappé notre joueur. Nous faisons cela en comparant les variables `meteor-x` et `player`. Si ce sont les mêmes, alors le météore a frappé le joueur et le jeu est perdu.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/06.png?raw=true">

Presque fini ! Nous voulons maintenant nous assurer que nous pouvons jouer jusqu'à ce qu'un météore touche le joueur. Pour se faire, nous utilisons une nouvelle variable `alive` et une boucle while.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/07.png?raw=true">

Il faut également faire les changements dans les mouvements de notre joueur.

<img src="https://github.com/serresebastien/Micro-Bit/blob/master/img/le-jeu-du-meteor/08.png?raw=true">

## Pour aller plus loin (1/2)

Ajouter une variable score et ajouter 1 à chaque fois qu'un météore est évité.
Montrez cette variable au lieu du X géant à la fin de la partie.

## Pour aller plus loin (2/2)

Maintenant que vous avez une variable de score, utilisez-la pour changer la durée du retard dans le code de chute de météores.
La pluie de météores commence lentement et devient plus rapide à mesure que la variable de score augmente.