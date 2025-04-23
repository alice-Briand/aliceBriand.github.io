---
title: Stage de deuxième année
publishDate: 2020-03-02 00:00:00
img: /aliceBriand.github.io/assets/stage2/endi.png
img_alt: Logo de Endi
description: |
  Amélioration du processus de facturation
tags:
  - Stage
  - Dev
  - PHP
  - JavaScript 
  - HTML
  - CSS
---

## But du stage

> Amélioration du processus de facturation

Lors de mon stage, j’ai créé un site web à partir des données d'une API. L'objectif de mon stage était de créer une visionneuse afin de faciliter le partage d’un devis ou d’une facture avec les clients.

### Mise en contexte

Endi est un logiciel libre développé par CAERP, qui permet de créer et de gérer des devis ainsi que des factures. Le problème était l’impossibilité, pour les clients, de modifier les prix dans le cas d’un prix conscient (le client estime le prix à payer pour la prestation).  
Pour contourner cette contrainte, il fallait d’abord créer un tableur, le faire valider ou modifier par le client, puis le recréer manuellement sur Endi — une méthode peu pratique et chronophage.

![page PDF d'un devis](/aliceBriand.github.io/assets/stage2/exempleDevis.png)

Pour faciliter ces étapes, j’ai créé une liseuse.

### Déroulement du stage

Lors de ce stage, j’ai tout d’abord commencé par mettre en place mon environnement de développement avec l’IDE PhpStorm, ainsi que XAMPP et un projet Git.

Ensuite, j’ai pris connaissance du code qui m’a été transmis et de mon objectif.  
J’ai également dû prendre en main l’API Endi sur Framagit grâce à un ticket listant les endpoints, car il n’y avait pas de documentation.

Pour gérer l’organisation, j’ai utilisé Git via des tickets, afin de mieux gérer les tâches et versionner le code.

![exemple de tickets Git](/aliceBriand.github.io/assets/stage2/tickets_Git.png)

Après cela, j’ai commencé à coder pour récupérer les données de l’API Endi et les afficher sur le site.  
Par la suite, j’ai ajouté un formulaire permettant de modifier le tarif horaire, puis un formulaire de connexion pour accéder à la liste des devis et des factures.

Enfin, nous avons déployé le site.

### Récupération des données

Lors de mon stage, j’ai d’abord commencé par créer la page en HTML et en PHP afin de pouvoir récupérer les données des devis via l’API et les afficher.

![page d'accueil d'un devis](/aliceBriand.github.io/assets/stage2/page1.png)

J’ai ensuite utilisé le CSS pour mettre en forme la page.

Une fois cela fait, j’ai également vérifié l’accessibilité et l’écoconception du site.

### Formulaire de prix conscient

J’ai ajouté, en haut de la page, un formulaire permettant de modifier le tarif horaire dans le cadre des prix conscients.

![formulaire de tarif horaire](/aliceBriand.github.io/assets/stage2/form_tarifHoraire.png)

J’ai mis en place un formulaire HTML permettant de modifier certaines données.  
Lors de la validation, un script JavaScript utilise l’API REST via la méthode `fetch()` avec la méthode `POST`, puis notre serveur envoie une requête en `PATCH` à l’API Endi afin de mettre à jour les informations côté serveur.  
Cette action entraîne également une mise à jour dynamique des données affichées sur la page, afin d’assurer la cohérence entre l’interface utilisateur et les données de l’API.

![méthode fetch](/aliceBriand.github.io/assets/stage2/methode_fetch.png)

### Formulaire de connexion

Pour le formulaire de connexion, j’ai utilisé la méthode `XHR` avec `POST` et `FormData`, ce qui permet d’envoyer les données du formulaire (ici, le mot de passe) à l’API pour valider la connexion.

![pop-up de connexion](/aliceBriand.github.io/assets/stage2/popUp_connexion.png)  
![méthode XHR](/aliceBriand.github.io/assets/stage2/methode_xhr_send.png)

Une fois la connexion validée, on affiche la liste des devis et des factures sous forme de liens de partage pour faciliter l’accès aux pages, ainsi qu’un bouton de déconnexion.

### Déploiement

Pour le déploiement, nous avons utilisé Infomaniak. Nous avons créé un sous-domaine, puis nous nous sommes connectés en SSH pour cloner le projet Git et ainsi récupérer le projet — ce qui permet de le mettre à jour automatiquement.

#### Compétences acquises / améliorées

- Langage JavaScript → `fetch` / `XHR` / `FormData`  
- Langage PHP  
- API REST  
- Git
