---
title: "Présentation de Gatsby Cloud"
description: "Présentation de la plateforme Gatsby Cloud."
date: "2021-05-28"
banner:
  src: "../../images/kelly-sikkema-Hl3LUdyKRic-unsplash.jpg"
  alt: "Image"
  caption: 'Photo by <u><a href="https://unsplash.com/photos/Nc5Q_CEcY44">Florian Olivo</a></u>'
categories:
  - "Gatsby"
  - "Cloud"
keywords:
  - "Example"
  - "Gatsby"
  - "Cloud"
  - "Blog"
---

## Code block test

```css
.AClass .Subtitle {
  margin: -0.5rem 0 0 0;
  font-weight: 700;
      font-size: 1.25rem;
  line-height: 1.5rem;
}

.AnotherClass p {
  font-size: 1.125rem;
  margin-bottom: 2rem;
}

.AThirdClass {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

@media (max-width: 768px) {
  .AClass {
    flex-direction: column;
  }
  .AnotherClass {
    display: block;
  }
}
```

Inline code: `print()`

 
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

Bien, maintenant faisons la même chose mais en passant cette fois ci par Gatsby Cloud. 
Il va falloir, dans un premier temps, comme sur tous les sites, vous créer un compte. Attention, ici, se connecter en utilisant son compte Github est, en plus d'être un gain de temps, un réel avantage (on va voir pourquoi dans 30 secondes). 

On peut alors commencer par créer notre site. Dans un premier temps il va nous être demandé si nous souhaitons importer un projet depuis notre github ou bien en commencer un nouveau utilisant les thèmes proposés par gatsby. Ici nous allons partir de zéro et donc sélectionner la deuxième option. Je vous conseille d'être vigiliant lors du choix du thème de départ car ceux-ci peuvent demander à être liés à des CMS, ce qui peut se montrer contraignant dans le cas où vous n'aviez pas prévu d'en utiliser.

Une fois notre thème sélectionné Gatsby Cloud va vous permettre de directement créer un repository Github pour votre site. C'est après cette étape que la magie va enfin opérer ! En effet, Gatsby va alors automatiquement vous **génerer un nom de domaine**, **build le projet** et le **mettre en ligne** ! Il va même par la suite s'occuper de faire la mise en production lorsqu'un changement surviendra dans le repository.  


## Utile ?

C'est bien joli tout cela, mais est-ce que c'est réellement utile, et si oui, à qui ?

Le framework Gatsby et son interface de gestion Gatsby Cloud semble viser les mêmes cibles, ce qui semble cohérent. 
Un public ayant des connaissances relativement solides en programmation web peut être intéressé par Gatsby. En effet, des technologies assez avancées sont utilisées par le framework, je pense nottamment à React ou à GraphQL, qui ne sont pas faciles à comprendre pour des néophites.

Cependant, c'est un framework qui est destiné à  la réalisation de sites relativement basiques et de petits projets. 

Il serait pertinant de l'utiliser pour créer des blogs, des portfolios ou des sites vitrines par exemple. 
Gatsby pourrait parfaitement convenir à des developpeurs freelance réalisant des sites simples. Gatsby cloud serait pour eux un réel avantage car cela leur permettrai de pouvoir gérer simplement et efficacement une multitude de site 
![This is the alt tag.](../../images/kelly-sikkema-Hl3LUdyKRic-unsplash.jpg "This is a markdown [caption](https://konstantin.digital).")


![This is the alt tag.](../../images/charles-deluvio-DgoyKNgPiFQ-unsplash.jpg)
