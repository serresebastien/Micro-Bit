---
title: 6- Les lucioles
nav_order: 6
---

# Les lucioles

## Objectif de la fiche

* Utiliser le module Bluetooth et les blocs Radio
* Savoir faire communiquer les Micro-bit entre eux
* Savoir définir puis faire appel à une fonction

## Première étape, allumer notre écran et envoyer un message

Le code ci-dessous, règle la luminosité au maximum, allume toutes les LED de l’écran, puis les éteint après une pause de 500 milliseconde lorsque l’on presse le bouton A.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/luciole/01.png?raw=true">

Nous aimerions en plus de tout ceci que notre Micro-bit envoie un message « boop » par bluetooth. Pour cela, rendez-vous dans la partie Radia et choisissez le bloc « send string ».

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/luciole/02.png?raw=true">

## Deuxième étape, recevoir et transmettre notre message

Attaquons-nous à la réception de notre message « boop ». Nous interrogeons notre carte pour savoir si un message équivalant à « boop » est reçu. Si tel est le cas, nous réglons la luminosité au maximum, allumons toutes les LED de l’écran, puis les éteignions après une pause de 500 milliseconde

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/luciole/03.png?raw=true">

Maintenant, afin que notre message communique aux cartes présentes aux alentours, nous allons renvoyer notre message « boop ». Afin de ne pas tomber dans une boucle infinie nous allons tirer un chiffre aléatoire en 0 et 3, si le chiffre est 3 alors nous envoyons notre message.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/luciole/04.png?raw=true">

## Troisième partie, rajoutons un peu d’aléatoire

Afin que notre programme paraisse plus naturel. Nous allons rajouter des délais d’attente aléatoire compris entre 50 et 500 millisecondes. Voici le bloc que nous allons utiliser :

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/luciole/05.png?raw=true">

Nous allons le mettre à deux endroits dans notre programme.

<img src="https://github.com/serresebastien/MicroBit/blob/master/img/luciole/06.png?raw=true">