# Brasilic

## Overview

Ce robot est un robot 6 DOF avec 3 joints horizontaux et 3 joints verticaux. La taille du robot est un peu supérieure à 60cm. 

A la base du robot il y a des emplacements pour un Arduino, un PCA9685 et un RaspberryPi (RPI5 pour une prochaine version).

Un passage de câble, le plus discret possible, est prévu à l'intérieur du robot depuis l'effecteur terminal jusqu'à la base.

L'axe 6 contient un socle pour accueillir un électro-aimant et des pogo pins pour permettre, dans des versions ultérieures, de changer d'effecteur terminal durant l'utilisation.
La base de l'effecteur terminal est encore à travailler pour connecter cette dernière au reste du robot.

L'effecteur terminal, une pince contrôlée par un 7e servo moteur, n'est pas présentée car achetée directement en magasin.

## Les servo : 

* Servomoteur 1 : Joint horizontal. Monté en prise directe. Présence de deux roulement : un 6804, pour le palonnier du moteur, et un 51108 à butée axiale pour supporter le poids. (Moteur 35kg/cm)
* Servomoteur 2 : Joint vertical. Action déportée. Présence d'un système de pignon courroie de ratio 1:2. Deux roulements 608 présent de part et d'autre du joint. (Servo 35kg/cm)
* Servomoteur 3 : Joint vertical. Action déportée. Présence d'un système de pignon courroie de ratio 1:2. Deux roulements 608 présent de part et d'autre du joint. (Servo 35kg/cm)
* Servomoteur 4 : Joint horizontal. Monté en prise directe. Présence de deux roulement : un 6804, pour le palonnier du moteur, et un 51108 à butée axiale pour supporter le poids. (Servo 25kg/cm)
* Servomoteur 5 : Joint vertical. Monté en prise directe. Un roulements 608 présent de l'autre côté du servo.(Servo 25kg/cm)
* Servomoteur 6 : Joint horizontal. Monté en prise directe. Présence de deux roulement : un 6804, pour le palonnier du moteur, et un 51108 à butée axiale pour supporter le poids.(Servo 25kg/cm)

## Configuration électrique :

L'alimentation de 5V 20A est la seule source d'énergie dans ce système. Pour alimenter les servos la tension de cette alimention a été augmentée à 6.7V et un abaisseur de tension est prévu pour pouvoir alimenter des composants comme le Arduino, le ventilateur à la base qui ont une tensions nominale de 5V. Une diode et un transistor sont aussi prévus pour le contrôle du ventilateur.

Deux câbles épais vont traverser le robot pour fournir de l'électricité aux composants. Les cables de commande (pwm des servos) vont eux, descendre jusqu'à la base.







