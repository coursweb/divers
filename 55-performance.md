---
layout: page
title: Performance
permalink: /performance/
---

Par "performance", on entend la rapidité de chargement et la réactivité d'un site. C'est un sujet passionnant et vaste, car d'innombrables facteurs entrent en jeu, autant au niveau du code frontend (chargement asynchrone), de la préparation des ressources (images, logos, fontes), du code serveur (systèmes de cache, optimisations diverses).

La question de la performance concerne aussi le graphisme du site, car les images, fontes typographiques et vidéos influent sur la vitesse de chargement - chaque donnée à un "coût" en terme de performance.

Lire à ce sujet l'article de Dan Mall: *[How To Make a Performance Budget](http://v3.danielmall.com/articles/how-to-make-a-performance-budget/)*.

## Outils et méthodes

- [Request Map](http://requestmap.webperf.tools/)  - dessine une arborescence des requêtes à divers domaines, effectués lors du chargement d'une page. Permet de détecter l'importance des connexions des scripts d'analytics, réseaux sociaux, etc.
- [WebPageTest](https://www.webpagetest.org/)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) - outil intégré dans les DevTools de Chrome.
- [Pagespeed Insights](https://developers.google.com/speed/pagespeed/insights/) - outil d'analyse de Google, donne un score à votre site et détecte des améliorations possibles. 
- [Pingdom](https://tools.pingdom.com/) (Website Speed Test)
- [GTmatrix](https://gtmetrix.com/)

Articles:

- *[Identifying, Auditing, and Discussing Third Parties](https://csswizardry.com/2018/05/identifying-auditing-discussing-third-parties/)*, CSS Wizardry. Décrit comment l'auteur analyse l'impact de "scripts tiers", à l'aide d'outils comme Request Map et WebPageTest... et comment il discute de l'utilité des scripts avec les équipes marketing.


## Technologies récentes

### Facebook Instant Articles et AMP

*Accelerated Mobile Pages* (AMP) est une technologie proposée par Google depuis 2015. Comme son nom l'indique, l'objectif est d'accéler le chargement de pages web, en particulier pour des appareils mobiles. La solution utilisée par Google proposer de créer des pages simplifiées, avec un CSS réduit au strict minimum, et une librairie JavaScript imposée par Google. Ces pages peuvent être montrées dans un carousel dans les résultats de recherche des navigateurs mobiles. Leurs contenus sont mises en cache par Google, ce qui permet un chargement "instantané" lorsqu'elles sont cliquées.

#### Controverse

Le lancement de AMP a provoqué des critiques: 
- Google n'a pas suivi la procédure habituelle pour proposer ce nouveau standard. Pour créer une page AMP il faut utiliser des propriétés inventées par Google, on crée donc du HTML non-valide.
- Google oblige les auteurs à anonymiser le contenu, la présentation visuelle étant uniformisée. Cela peut renforcer le phénomène des "fake news": des fausses infos vont paraître légitimées, car apparaissant dans les *news* mises en avant par Google.
- La performance d'une page AMP n'est pas meilleure qu'une page web bien optimisée. La vitesse vient en fait du "pré-chargement" des ressources effectué par GOogle.

Quelques articles critiques: 

- Jeremy Keith, *[The meaning of AMP](https://adactio.com/journal/13035)*, 2017
- Scott Gilbertson, [Kill Google AMP before it kills the web](https://www.theregister.co.uk/2017/05/19/open_source_insider_google_amp_bad_bad_bad/), The Register, 2017
- Ferdy Christant, *[AMP: the missing controversy](https://ferdychristant.com/amp-the-missing-controversy-3b424031047)*, 2018


> "One of the reasons why AMP first appeared to be different to *Facebook Instant Articles* or *Apple News* was the promise that you could host your AMP pages yourself. That’s the very reason I first got interested in AMP. But if you actually want the benefits of AMP — appearing in the not-search-results carousel, pre-rendered performance, etc. — then your pages must be hosted by Google." – Jeremy Keith

#### Documentation

* [Le site officiel du projet AMP](https://amp.dev/)



### Progressive Web Apps (PWA)

Par Progressive Web App (PWA), on décrit une technologie qui permet à un site web de bénéficier de certaines fonctionnalités réservées jusqu'ici aux applications mobiles. Notamment:

- Charger du contenu qui restera accessible même sans connexion internet.
- Installer un raccourci sur l'écran de l'appareil.
- Proposer des "push notifications".
- Accéder à des API du système.
- Accéder au hardware de l'appareil.

> Google has been spearheading the movement to enhance web applications by converting them to progressive web apps (PWA’s), and 2017 has seen a rapid adoption. A PWA utilizes modern browser technologies to provide a web experience that is more like mobile applications. This offers improved performance and offline experience as well as features previously only available to mobile, such as push notifications. The backbone for PWA’s are a combination of a manifest.json file and utilizing service workers. – Trey Huffine, [A recap of front-end development in 2017](https://levelup.gitconnected.com/a-recap-of-front-end-development-in-2017-7072ce99e727)

Au sujet des "PWA", Jeremy Keith a publié en 2018 le livre "[Going Offline](https://abookapart.com/products/going-offline)" chez l'éditeur "A Book Apart".

Conférence de Jeremy Keith, mai 2018 : [https://noti.st/adactio/d1zSa7](https://noti.st/adactio/d1zSa7)

Exemples de Progressive Web Apps:

* [YouTube Music](https://music.youtube.com/), par Google
* [Spotify](https://open.spotify.com/)
* [Twitter](https://twitter.com/)
