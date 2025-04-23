---
title: Ministages
publishDate: 2020-03-04 00:00:00
img: /aliceBriand.github.io/assets/Ministage/logo_ministage.jpg
img_alt: Logo du site Ministage
description: |
  Mettre à jour et améliorer une application web
tags:
  - Dev
  - PHP
  - Groupe
  - Symfony
  - Framagit
---

## Objectif du projet

> Mettre à jour une application web et l'améliorer.

Pour ce projet, nous avons récupéré une application réalisée par un stagiaire en 2015.  
Nous avons travaillé avec notre porteur de projet, M. Mordelet. Le but du projet était de corriger les bugs, de mettre à jour et d'améliorer le site (création d'une version Symfony).  
<br></br>

![page de login](/aliceBriand.github.io/assets/Ministage/login_ministage.png)

### Contexte

Ministage44 est un site web réalisé par un stagiaire en 2015. Il permet à des élèves de collège ou de lycée d’effectuer des ministages dans des établissements, dans le but de découvrir de nouvelles formations.

### Organisation du travail

Pour ce projet, nous avons utilisé la méthode agile, ce qui impliquait de présenter régulièrement nos avancées à notre porteur de projet.

Nous avons commencé par installer notre environnement de travail :  
nous avons utilisé **XAMPP** pour avoir la bonne version de PHP, ainsi que l’IDE **PhpStorm** et **DBeaver** pour accéder à la base de données.

La première semaine a été consacrée à la prise de connaissance du code et de l’architecture du site. Répartis en groupes, chacun s’est chargé de l’un des 4 profils de connexion.  
Mon groupe s’est occupé du profil **Consultation**, ce qui nous a permis de bien comprendre le fonctionnement de Ministage44. Nous avons ensuite présenté ce que nous avions compris au porteur de projet.

![cartographie de l'application](/aliceBriand.github.io/assets/Ministage/cartographie.png)

Après ce premier sprint, nous avons commencé à coder et à corriger les bugs existants.

Puis, nous avons entamé le développement d’une nouvelle version de Ministage44 sous Symfony.

### Partage des tâches

Pour le partage des tâches, nous avons créé des tickets répertoriant les bugs (plus ou moins critiques) ainsi que les améliorations à apporter, sur le dépôt Git du projet.  
Nous nous sommes répartis les différentes tâches à réaliser, seuls ou en petits groupes.

![ticket git](/aliceBriand.github.io/assets/Ministage/ticket.png)

### Correction de bugs

Tout au long de l’année, nous avons corrigé de nombreux bugs signalés par notre porteur de projet.  
Par exemple, l’envoi de mails ne fonctionnait pas, ce qui ne répondait pas aux attentes des utilisateurs.

Pour cela, nous choisissions un ticket disponible, identifions le problème dans le code, puis proposions une solution pour le résoudre.

Après chaque correction, nous avions une rencontre avec notre porteur de projet pour lui présenter nos modifications et procéder au déploiement.

### Symfony

Après avoir résolu la majorité des problèmes du site, une partie de la classe s’est lancée dans le développement d’une nouvelle version de Ministage44 à l’aide du framework **Symfony**.

Cela nous a permis de repartir de zéro, afin de réécrire le code de manière plus claire et de refondre la base de données, qui présentait plusieurs problèmes.

Pour la répartition du travail, nous avons créé un nouveau dépôt Git avec de nouveaux tickets. Par petits groupes, nous avons développé les **contrôleurs** ainsi que les **vues**.

Nous avons également recréé une **page de connexion** et mis en place une **gestion des accès** sur les routes.

## Compétences

Compétences travaillées lors de ce projet :

- PHP  
- Git  
- Travail en groupe  
- Symfony
