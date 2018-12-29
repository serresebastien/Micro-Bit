---
title: 1- Présentation de la carte
nav_order: 1
---

# Introduction à la carte Micro-bit

## Objectif de la fiche

* Évaluer le niveau de connaissance de chaque enfant
* Amener les enfants à réfléchir sur les éléments constituant un ordinateur
* Familiariser l’enfant avec l’interface de programmation
* Créer et téléverser notre premier programme

## Première activité

Notre première activité consiste à introduire la carte de programmation Micro-bit que nous allons utiliser par la suite. Pour ce faire, avant de donner les cartes Micro-bit aux enfants, interrogez l’ensemble du groupe sur les composants qui constitue un ordinateur d’après eux.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/01.png?raw=true">
                     
Quelques éléments de réponse
* Un processeur
* Des périphériques d’entrées (souris, clavier, webcam...)
* Des périphériques de sorties (écran, imprimante, haut-parleur...)
* Une batterie
* Des interfaces de connexion (port USB, Bluetooth...)

Une fois l’activité terminée, distribuez les cartes Micro-bit aux enfants et laissez-les interagir avec. Faites-les chercher les différents composants cités plus haut sur la carte.

## Deuxième activité

Maintenant que les présentations entre la carte Micro-bit et les enfants sont faites, passons à l’interface de programmation nous permettant de coder nos programmes à destination de notre carte Micro-bit.

Demandez aux enfants d’ouvrir un navigateur internet et de se rendre sur le site de Micro-bit : [microbit.org](https://microbit.org/). Une fois sur le site, rendez-vous dans « Viens Coder ! », vous arrivez sur une nouvelle page : le *JavaScript Block Editor*.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/02.png?raw=true">

Voici à quoi ressemble notre interface de programmation. Intéressons-nous aux différentes parties de l’éditeur :

<span style="color:green; font-weight:bold">En vert :</span> Un espace de visualisation en direct de l’effet de notre code sur la carte Micro-bit. Cela est très pratique et nous permettra de tester notre programme sans avoir besoin de le téléverser sur notre carte.
Les différentes icônes en dessous de la carte permettent dans l’ordre d’arrêter la simulation, de redémarrer la simulation, de ralentir la vitesse de la simulation, d’activer/désactiver le son et de visualiser la simulation en plein écran.

<span style="color:gold">**En jaune :**</span> C’est ici que tous les blocs nous permettant de concevoir nos programmes se trouvent. Ils sont classés par catégories et chacune d’entre elle à couleur qui lui est propre. Une barre de recherche en haut nous permet trouver un élément en quelques secondes.

<span style="color:red">**En rouge :**</span> Voici notre terrain de jeu. C’est ici que nous construisons nos programmes en y plaçant les blocs obtenus dans le menu. 

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/03.png?raw=true">

Intéressons-nous au menu en bas de page. Ce dernier permet de gauche à droite, réduire l’espace de la simulation, télécharger le programme que nous venons de réaliser au format .hex, donner un nom à notre programme, d’annuler la dernière action effectuée, ré effectuer l’action précédemment annulée et de zoomer ou dézoomer sur notre espace de programmation.

## Troisième activité

C’est le moment de programmer notre premier projet ! Ce premier programme permet aux enfants de s’exercer avec la prise en main de l’interface de programmation.

Notre programme permet simplement d’afficher des icônes sur l’écran de notre Micro-bit. Nous allons exclusivement utiliser les blocs présents dans la partie « Basique » (en bleu).

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/04.png?raw=true">

Notre programme se déroule en deux étapes. La première se déroule une fois la carte sous tension et la deuxième se déroule sans cesse une fois la première terminée.

Pour se faire, nous allons utiliser deux blocs « au démarrage » et «toujours». Ces deux blocs sont différents des autres, il faut y placer des blocs à l’intérieur.
Laissez les enfants s’approprier les blocs. Proposez-leur de faire un programme qui affiche des icônes au démarrage puis leur prénom suivi de leur âge indéfiniment.

Voici une proposition de réponse, bien entendu il n’y a pas de réponse exacte, celle-ci est donnée à titre d’exemple.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/05.png?raw=true">

Le programme ci-dessus, affiche au démarrage un cœur puis le texte suivant indéfiniment :
```
Bonjour,
Je m’appelle Tom.
J’ai 11 ans.
```
Maintenant que notre code est réalisé, il nous reste à le téléverser sur notre carte Micro-bit. En bas de l’interface de programmation, donnez un nom à notre programme, par exemple « hello » puis cliqué sur le bouton « Télécharger ».

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/06.png?raw=true">

Une fois le fichier *microbit-hello.hex* téléchargé sur l’ordinateur, connecté la carte Micro-bit à l’ordinateur via le câble USB fourni dans la boite et placer le fichier dans le Micro-bit (un simple glissé déposé ou un copier/coller suffit).

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/introduction/07.png?raw=true">

Vous pouvez télécharger le programe ci dessus ici : <a href="https://raw.githubusercontent.com/serresebastien/MicroBit/master/code/microbit-hello.hex">microbit-hello.hex</a>