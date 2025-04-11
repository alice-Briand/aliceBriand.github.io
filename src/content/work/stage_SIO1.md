---
title: Stage de première année
publishDate: 2020-03-02 00:00:00
img: /aliceBriand.github.io/assets/stage/logo-pole_sante-noir.jpg
img_alt: Logo du pôle sante de Nantes Université
description: |
  Migration d'une application
tags:
  - Stage
  - Dev
  - PHP
---

## But du stage

> Migration d'une application plus ajout d'une function.

Lors de mon stage, je travaille sur une application en PHP qui permet d'envoyer des mails de convocation pour surveiller des examens. L'objectif de mon stage est donc que je migre cette applicatin sur un nouveau serveur ainsi que rajouter une fonction. Pour cela je dois d'abord verifier 

[Lien vers l'application](https://surveillance.sante.univ-nantes.fr/)

![page d'accueil du site](/aliceBriand.github.io/assets/stage/accueil_surveillance2.1.PNG)

### Déroulement du stage

Lors de se stage, j'ai tout d'abord commencé par mettre en place mon environnement de developpement en installant un IDE puis un debuggeur PHP, ainsi que un lien Git.

Ensuite, j'ai pris connaissance du code, d'une application déjâ faite, que l'on m'a transmit. Puis j'ai réalisé des tests unitaire afin de voir si le le code fonctionnais toujours.

Et après cela, j'ai remplacé la fonction de mail avec phpMailer et j'ai rajouté un fichier .ics.

### Tester les classes

Lors de mon stage j'ai d'abord commencé par faire des pages de test sur les classe afin de savoir si celci fonctionnais toujours sachant que l'application était en PHP 5 et que depuis PHP 7 certaines fonction sont obselette et mysql ne fonctionne plus non plus.

![page de test](/aliceBriand.github.io/assets/stage/pageTest1Modif.PNG)
J'ai donc créé plusieurs test en PHP dans le but de testé les méthodes comme dans l'exemple ci dessus avec la classe Surveillance.

Une fois les test fait, je lance un script qui les executes et qui affiche le résultat, comme ci dessous.
![page de test](/aliceBriand.github.io/assets/stage/resultat_testModif.PNG)

J'ai fait face à differentes erreurs, comme ci-dessous, que j'ai du corrigé.
![erreur, pas autant d'argument donné que demandé](/aliceBriand.github.io/assets/stage/exemple_erreur1.PNG)
![valeur de sortie differrente de celle attendu](/aliceBriand.github.io/assets/stage/exemple_erreur2.PNG)

Et j'ai parfois du modifier le code principale car celui-ci ne fonctionnais pas 
![function modifier](/aliceBriand.github.io/assets/stage/code_modifier1.PNG)
![function modifier](/aliceBriand.github.io/assets/stage/code_modifier.PNG)
Dans l’exemple ci-dessus, le code ne fonctionnais pas car le code essayait d’exécuter deux requêtes en même temps. J’ai donc refait le code en effectuant les deux requêtes séparément.



### Envoie des mails

Après avoir effectué les différents tests, j'ai modifier les pages d'envoie de mail.
pour envoyer des mail j'ai utilisé phpMailer et j'ai donc écrit le code dont j'avais besoin.
![code de PHPMailer](/aliceBriand.github.io/assets/stage/PHPMailer.PNG)

Une fois que l'envoie des mails fonctionnais, j'ai rajouté un fichier .ics, ce qui permet d'avoir un lien qui met directement l'evenement du mail dans l'agenda lorsque ont l'ouvre.
![code de fichier .ics](/aliceBriand.github.io/assets/stage/ics0.PNG)



#### Compétences aquises

- language PHP -> test
- travail en condition réel


