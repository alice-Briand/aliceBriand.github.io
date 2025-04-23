---
title: Stage de première année
publishDate: 2020-03-02 00:00:00
img: /aliceBriand.github.io/assets/stage/logo-pole_sante-noir.jpg
img_alt: Logo du pôle santé de Nantes Université
description: |
  Migration d'une application
tags:
  - Stage
  - Dev
  - PHP
---

## But du stage

> Migration d'une application et ajout d'une fonctionnalité.

Lors de mon stage, j’ai travaillé sur une application en PHP permettant d’envoyer des mails de convocation pour surveiller des examens.  
L’objectif de mon stage était donc de migrer cette application vers un nouveau serveur, ainsi que d’ajouter une nouvelle fonctionnalité.  
Pour cela, j’ai d’abord dû vérifier le bon fonctionnement du code.

[Lien vers l'application](https://surveillance.sante.univ-nantes.fr/)

![page d'accueil du site](/aliceBriand.github.io/assets/stage/accueil_surveillance2.1.PNG)

### Déroulement du stage

Lors de ce stage, j’ai d’abord mis en place mon environnement de développement en installant un IDE, un débogueur PHP, ainsi qu’un lien Git.

Ensuite, j’ai pris connaissance du code d’une application déjà existante, qui m’a été transmise.  
J’ai ensuite réalisé des tests unitaires afin de vérifier que le code fonctionnait toujours correctement.

Par la suite, j’ai remplacé la fonction d’envoi de mails par **phpMailer**, et j’ai ajouté la génération d’un fichier **.ics**.

### Tests des classes

J’ai commencé par créer des pages de test sur les classes pour vérifier leur bon fonctionnement, sachant que l’application était en PHP 5 et que, depuis PHP 7, certaines fonctions sont devenues obsolètes.  
De plus, `mysql` n’est plus pris en charge.

![page de test](/aliceBriand.github.io/assets/stage/pageTest1Modif.PNG)

J’ai donc créé plusieurs tests en PHP dans le but de tester les méthodes, comme dans l’exemple ci-dessus avec la classe **Surveillance**.

Une fois les tests créés, je lançais un script qui les exécutait et affichait les résultats :

![page de test](/aliceBriand.github.io/assets/stage/resultat_testModif.PNG)

J’ai rencontré différentes erreurs, comme celles ci-dessous, que j’ai dû corriger :

![erreur, pas autant d'arguments donnés que demandés](/aliceBriand.github.io/assets/stage/exemple_erreur1.PNG)  
![valeur de sortie différente de celle attendue](/aliceBriand.github.io/assets/stage/exemple_erreur2.PNG)

Parfois, j’ai même dû modifier le **code principal** car certaines parties ne fonctionnaient pas :

![fonction modifiée](/aliceBriand.github.io/assets/stage/code_modifier1.PNG)  
![fonction modifiée](/aliceBriand.github.io/assets/stage/code_modifier.PNG)

Dans cet exemple, le code ne fonctionnait pas car il essayait d’exécuter deux requêtes SQL en même temps.  
J’ai donc modifié le code pour effectuer les deux requêtes séparément.

### Envoi des mails

Après avoir effectué les différents tests, j’ai modifié les pages d’envoi de mails.  
Pour cela, j’ai utilisé **phpMailer** et réécrit le code nécessaire.

![code de PHPMailer](/aliceBriand.github.io/assets/stage/PHPMailer.PNG)

Une fois l’envoi des mails fonctionnel, j’ai ajouté un fichier **.ics** (fichier d’agenda).  
Cela permet d’avoir un lien dans le mail qui ajoute directement l’événement dans l’agenda du destinataire.

![code du fichier .ics](/aliceBriand.github.io/assets/stage/ics0.PNG)

## Compétences acquises

- Langage PHP → Tests unitaires, maintenance de code existant  
- Travail en condition réelle (application en production)
