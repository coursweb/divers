---
layout: page
title: Performance
permalink: /divers/performance/
---

Par "performance", on entend la rapidité de chargement et la réactivité d'un site. C'est un sujet passionnant et vaste, car d'innombrables facteurs entrent en jeu, autant au niveau du code frontend (chargement asynchrone), de la préparation des ressources (images, logos, fontes), du code serveur (systèmes de cache, optimisations diverses).

La question de la performance concerne aussi le graphisme du site, car les images, fontes typographiques et vidéos influent sur la vitesse de chargement - chaque donnée à un "coût" en terme de performance.

Lire à ce sujet l'article de Dan Mall: *[How To Make a Performance Budget](http://v3.danielmall.com/articles/how-to-make-a-performance-budget/)*.

## Outils et méthodes

- [Request Map](http://requestmap.webperf.tools/)  - dessine une arborescence des requêtes à divers domaines, effectués lors du chargement d'une page. Permet de détecter l'importance des connexions des scripts d'analytics, réseaux sociaux, etc.
- WebPageTest

Articles:

- *[Identifying, Auditing, and Discussing Third Parties](https://csswizardry.com/2018/05/identifying-auditing-discussing-third-parties/)*, CSS Wizardry. Décrit comment l'auteur analyse l'impact de "scripts tiers", à l'aide d'outils comme Request Map et WebPageTest... et comment il discute de l'utilité des scripts avec les équipes marketing.


## Technologies récentes

### Facebook Instant Articles et AMP

Accelerated Mobile Pages est une technologie proposée par Google.

Lire: Jeremy Keith, *[The meaning of AMP](https://adactio.com/journal/13035)*, 2017

> "One of the reasons why AMP first appeared to be different to Facebook Instant Articles or Apple News was the promise that you could host your AMP pages yourself. That’s the very reason I first got interested in AMP. But if you actually want the benefits of AMP — appearing in the not-search-results carousel, pre-rendered performance, etc. — then your pages must be hosted by Google." – Jeremy Keith



### Progressive Web Apps

Permet de proposer du contenu qui restera accessible même sans connexion internet.

> Google has been spearheading the movement to enhance web applications by converting them to progressive web apps (PWA’s), and 2017 has seen a rapid adoption. A PWA utilizes modern browser technologies to provide a web experience that is more like mobile applications. This offers improved performance and offline experience as well as features previously only available to mobile, such as push notifications. The backbone for PWA’s are a combination of a manifest.json file and utilizing service workers. – Trey Huffine, [A recap of front-end development in 2017](https://levelup.gitconnected.com/a-recap-of-front-end-development-in-2017-7072ce99e727)

Au sujet des "PWA", Jeremy Keith a publié le livre "Going Offline" chez l'éditeur "A Book Apart".

Conférence de Jeremy Keith, mai 2018 : [https://noti.st/adactio/d1zSa7](https://noti.st/adactio/d1zSa7)