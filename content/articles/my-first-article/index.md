---
title: "Présentation du Framework Gatsby"
description: "Présentation du Framework GatsbyJs "
date: "2023-01-01"
banner:
  src: "../../images/kelly-sikkema-Hl3LUdyKRic-unsplash.jpg"
  alt: "Image"
  caption: 'Photo by <u><a href="https://unsplash.com/photos/Nc5Q_CEcY44">Florian Olivo</a></u>'
categories:
  - "Gatsby"
  - "Framework"
keywords:
  - "Veille!!"
  - "Gatsby"
  - "Framework"
  - "Presentation"
---

## Le framework gatsby

Tout comme je l'ai expliqué sur la page d'introduction, la promesse du framework gatsby est de faciliter la mise en place de sites statiques, tout en promettant leur sécurité et leur rapidité. L'objectif est également de combiner plusieurs technologies afin de pouvoir créer de beaux sites pouvant répondre à un maximum de besoins.

Pour cela, gatsby intègre nativement ReactJs, Markdown et GraphQl. Ensuite, libre à nous de les utiliser ou non. 
Lors de la création de notre site en ligne de commandes, ```npm init gatsby``` il est possible de préciser si on souhaite que TypeScript soit mit à la place de JavaScript dans les fichiers de départ de Gatsby.

L'utilisation de Markdown peut notamment permettre au développeur de déléguer la gestion du contenu au client ou autre. 

Gatsby propose par ailleurs un système de plugins permettant d'ajouter des fonctionnalités facilement. 
```sh
npm install gatsby-plugin-material-ui@next @emotion/react
```
La commande ci-dessus permet d'utiliser MaterialUi. 
Gatsby met ainsi à disposition une documentation pour chacun de ces plugins indiquant comment les installer et les utiliser.
Parmi ces plugins, il y a un grand nombre de CMS (Contentful, WordPress, Drupal, Sanity) mais également des plugins permettant la gestion de payements/e-commerce (Shopify) ainsi que des plugins d'UI et de CSS (Material UI, PostCSS, Emotion).

Cette diversité et ce grand nombre de fonctionnalités/plugins peut au final venir nous faire oublier que nous sommes sur un site statique. 

```js
import * as React from "react"
import { Link } from "gatsby"
import { StaticImage } from "gatsby-plugin-image"

import Layout from "../components/layout"
import Seo from "../components/seo"
import * as styles from "../components/index.module.css"

const links = [
  {
    text: "Tutorial",
    url: "https://www.gatsbyjs.com/docs/tutorial",
    description:
      "A great place to get started if you're new to web development. Designed to guide you through setting up your first Gatsby site.",
  },
  {
    text: "Examples",
    url: "https://github.com/gatsbyjs/gatsby/tree/master/examples",
    description:
      "A collection of websites ranging from very basic to complex/complete that illustrate how to accomplish specific tasks within your Gatsby sites.",
  },
  {
    text: "Plugin Library",
    url: "https://www.gatsbyjs.com/plugins",
    description:
      "Learn how to add functionality and customize your Gatsby site or app with thousands of plugins built by our amazing developer community.",
  },
  {
    text: "Build and Host",
    url: "https://www.gatsbyjs.com/cloud",
    description:
      "Now you’re ready to show the world! Give your Gatsby site superpowers: Build and host on Gatsby Cloud. Get started for free!",
  },
]

const samplePageLinks = [
  {
    text: "Page 2",
    url: "page-2",
    badge: false,
    description:
      "A simple example of linking to another page within a Gatsby site",
  },
  { text: "TypeScript", url: "using-typescript" },
  { text: "Server Side Rendering", url: "using-ssr" },
  { text: "Deferred Static Generation", url: "using-dsg" },
]

const moreLinks = [
  { text: "Join us on Discord", url: "https://gatsby.dev/discord" },
  {
    text: "Documentation",
    url: "https://gatsbyjs.com/docs/",
  },
  {
    text: "Starters",
    url: "https://gatsbyjs.com/starters/",
  },
  {
    text: "Showcase",
    url: "https://gatsbyjs.com/showcase/",
  },
  {
    text: "Contributing",
    url: "https://www.gatsbyjs.com/contributing/",
  },
  { text: "Issues", url: "https://github.com/gatsbyjs/gatsby/issues" },
]

const utmParameters = `?utm_source=starter&utm_medium=start-page&utm_campaign=default-starter`

const IndexPage = () => (
  <Layout>
    <div className={styles.textCenter}>
      <StaticImage
        src="../images/example.png"
        loading="eager"
        width={64}
        quality={95}
        formats={["auto", "webp", "avif"]}
        alt=""
        style={{ marginBottom: `var(--space-3)` }}
      />
      <h1>
        Welcome to <b>Gatsby!</b>
      </h1>
      <p className={styles.intro}>
        <b>Example pages:</b>{" "}
        {samplePageLinks.map((link, i) => (
          <React.Fragment key={link.url}>
            <Link to={link.url}>{link.text}</Link>
            {i !== samplePageLinks.length - 1 && <> · </>}
          </React.Fragment>
        ))}
        <br />
        Edit <code>src/pages/index.js</code> to update this page.
      </p>
    </div>
    <ul className={styles.list}>
      {links.map(link => (
        <li key={link.url} className={styles.listItem}>
          <a
            className={styles.listItemLink}
            href={`${link.url}${utmParameters}`}
          >
            {link.text} ↗
          </a>
          <p className={styles.listItemDescription}>{link.description}</p>
        </li>
      ))}
    </ul>
    {moreLinks.map((link, i) => (
      <React.Fragment key={link.url}>
        <a href={`${link.url}${utmParameters}`}>{link.text}</a>
        {i !== moreLinks.length - 1 && <> · </>}
      </React.Fragment>
    ))}
  </Layout>
)

/**
 * Head export to define metadata for the page
 *
 * See: https://www.gatsbyjs.com/docs/reference/built-in-components/gatsby-head/
 */
export const Head = () => <Seo title="Home" />

export default IndexPage
```


Le code que vous voyez ci-dessus est le code de la page d'index.js du starter par défaut de Gatsby.
Les autres starters ont, dans la globalité, les pages codées de la même manière que ci-dessus. 

Cette manière de rédiger (stocker les contenus, afficher dans des tableaux en haut de page) permet au contenu d'être visible et facilement modifiable, pas besoin d'être développeur pour apporter des modifications.

Cependant, si on veut modifier l'apparence du contenu, cela devient tout de suite bien plus fastidieux. En effet, comme tout le contenu est renseigné dans les tableaux en haut de page, le reste du code est brut et difficile à déchiffrer pour des non initiés.


![This is the alt tag.](../../images/charles-deluvio-DgoyKNgPiFQ-unsplash.jpg)
