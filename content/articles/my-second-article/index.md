---
title: "Présentation de Gatsby Cloud"
description: "Présentation de la plateforme Gatsby Cloud"
date: "2002-01-01"
banner:
  src: "../../images/cloud.jpeg"
  alt: "Image"
  caption: 'Photo by <u><a href="https://unsplash.com/photos/Nc5Q_CEcY44">Moi</a></u>'
categories:
  - "Gatsby"
  - "Cloud"
keywords:
  - "Veille!!"
  - "Gatsby"
  - "Cloud"
  - "Presentation"
---

Le framework Gatsby possède un atout de taille face à la concurrence. En effet, un service de Cloud est proposé à l'utilisateur, Gatsby Cloud (pourquoi faire compliquer !) . 
Gatsby Cloud se présente sous forme de site web permettant à l'utilisateur de gérer son site sans passer par les commandes fastidieuses en bash.

Afin de vous faire un inventaire des fonctionnalités importantes, je vais simuler avec vous le cycle de vie d'un site avec Gatsby Cloud.

Pour lancer un projet avec le framework gatsby, on peut utiliser les commandes basiques données dans la documentation :
```
npm init gatsby
cd my-gatsby-site
npm run develop
```
A la suite de ces trois commandes nous pouvons déjà avoir un site tournant sur le localhost.

Bien, maintenant faisons la même chose mais en passant cette fois-ci par Gatsby Cloud. 
Il va falloir, dans un premier temps, comme sur tous les sites, vous créer un compte. Attention, ici, se connecter en utilisant son compte Github est, en plus d'être un gain de temps, un réel avantage (on va voir pourquoi dans 30 secondes). 

On peut alors commencer par créer notre site. Dans un premier temps il va nous être demandé si nous souhaitons importer un projet depuis notre github ou bien en commencer un nouveau utilisant les thèmes proposés par gatsby. Ici nous allons partir de zéro et donc sélectionner la deuxième option. Je vous conseille d'être vigilant lors du choix du thème de départ car ceux-ci peuvent demander à être liés à des CMS, ce qui peut se montrer contraignant dans le cas où vous n'aviez pas prévu d'en utiliser.

Une fois notre thème sélectionné Gatsby Cloud va vous permettre de directement créer un repository Github pour votre site. C'est après cette étape que la magie va enfin opérer ! En effet, Gatsby va alors automatiquement vous **générer un nom de domaine**, **build le projet** et le **mettre en ligne** ! Il va même par la suite s'occuper de faire la mise en production lorsqu'un changement surviendra dans le repository.  

La centralisation de toutes ces fonctionnalités au travers de Gatsby Cloud nous permet concrètement de créer et déployer un site en 2 minutes chrono avec les mains dans les poches, comme en atteste la vidéo ci-dessous.    

[![Demo Gatsby](https://img.youtube.com/vi/VRYbtfbiJ64/0.jpg)](https://www.youtube.com/watch?v=VRYbtfbiJ64)
