---
title: Stage de deuxieme année
publishDate: 2020-03-02 00:00:00
img: assets/stage2/endi.png
img_alt: Logo du pôle sante de Nantes Université
description: |
  Migration d'une application
tags:
  - Stage
  - Dev
  - PHP
  - JavaScript 
  - HTML
  - CSS
---

## But du stage

> Création d'une visionneuse 

Lors de mon stage, J'ai créer un site web à partir des données d'une API. L'objectif de mon stage est donc de créer un visionneuse dans le but de faciliter le partage d'un devis ou d'une facture aux clients. 

### Mis en contexte

Endi est un site permettant de créer et gérer des devis et des factures. Le probleme est que sur le document PDF du devis à envoyer il y a un filigrame.
Pour eviter ça, il fallait faire un tableau exel, demander la validation du client puis le refaire sur endi ce qui n'était pas pratique.
![page PDF d'un devis](/public/assets/stage2/exempleDevis.PNG)
pour faciliter les étapes, j'ai du créer une liseuse.

### Déroulement du stage

Lors de se stage, j'ai tout d'abord commencé par mettre en place mon environnement de developpement avec l'IDE PhpStorm ainsi que xamp et un projet git.

Ensuite, j'ai pris connaissance du code que l'on m'a transmit, et de mon objectif.

Pour gérer l'organisatin j'ai utilisé Git grace aux tickets pour permettre une meilleure gestion des taches.
![exemple de tickets Git](/public/assets/stage2/tickets_Git.png)

Et après cela, j'ai commencé à code pour recuperer les données de l'API endi pour pouvoire les afficher sur le site. Puis j'ai rajouté un 

### Recupération des données

Lors de mon stage j'ai d'abord commencé par créer la page en HTML ainsi qu'en PHP afin de pouvoire récuperer les données des devis de l'API et de les afficher.

![page d'accueil d'un devis'](/public/assets/stage2/page1.PNG)

Et avec le CSS j'ai mis en forme la page.

Une fois fait, j'ai également vérifier l'accessibilité et l'écoconception du site.
![ecoconception](/public/assets/)
![accesibilité](/public/assets/)

### Formulaire de prix concient

J'ai ajouté, en haut de la page, un formulaire permetant de modifier les tarif horaire pour les prix concients

![code de PHPMailer](/public/assets/stage2/form_tarifHoraire.PNG)

J’ai mis en place un formulaire en HTML permettant de modifier certaines données.
Lors de la validation, un script JavaScript utilise l’API REST via la méthode fetch() avec la méthode PATCH, afin de mettre à jour les informations côté serveur.
Cette action entraîne également la mise à jour dynamique des données affichées sur la page, afin d'assurer une cohérence entre l’interface utilisateur et les données de l’API.
![code de fichier .ics](/public/assets/stage2/popUp_connexion.PNG)



#### Compétences aquises

- language PHP -> test
- travail en condition réel