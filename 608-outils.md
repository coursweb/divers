---
layout: page
title: Outils de développement web
permalink: /divers/outils/
---

> "Tools are dangerous - they can give you the illusion of knowing what you're doing." @p3ob7o at #wcch

Cet article présente une liste d'outils et logiciels utiles pour le design et la programmation web. 

Editeurs de code:
===

* *[TextWrangler](http://www.barebones.com/products/TextWrangler/)* - éditeur gratuit 
* *[Sublime Text](https://www.sublimetext.com/)* - éditeur gratuit, le plus populaire en ce moment. Il existe [un grand nombre d'extensions](https://packagecontrol.io/) pour étendre ses fonctionalités. 
* *[Atom](https://atom.io/)* - éditeur gratuit et open source, très similaire à Sublime Text. Il existe également [des extensions](https://atom.io/packages).
* *[Coda](https://panic.com/coda/)* - éditeur avec des fonctions de prévisualisation. Prix: $99.
* *[Espresso](http://www.macrabbit.com/espresso/)* - éditeur avec des fonctions de prévisualisation du CSS. Prix: $75. Développement en standby depuis juin 2015.
* *[PhpStorm](https://www.jetbrains.com/phpstorm/)* - éditeur spécialisé pour le langage PHP (utile pour le développement de thèmes WordPress, par exemple).

Parmi les fonctionalités partagées par tous ces éditeurs de code: 

- la colorisation de la syntaxe pour faciliter la lecture et la détection d’erreurs.
- la suggestion de termes propres au langage utilisé (HTML, CSS, JavaScript, etc).
- le  « rechercher remplacer » à l'échelle d'un projet ou dossier.
- le « rechercher remplacer » avec des « expressions régulières ».

**L'inspecteur du navigateur** est un outil indispensable pour le développement d'interfaces web. Il permet l’analyse des éléments de mise en page d’un site, son chargement, son poids etc. Il est disponible dans les navigateurs majeurs (Firefox, Chrome, Safari). À noter que Firefox propose une "[version développeur](https://www.mozilla.org/fr/firefox/developer/)".

Dans Safari, il est nécessaire d'activer ces outils dans les préférences (sous *Avancées > Afficher le menu Développement...*).

Afin de pouvoir tester des sites sous Internet Explorer, Microsoft propose des images virtuelles Windows incluant ce navigateur.



Statistiques & outils d'analyse
===

- *[Can I Use](http://caniuse.com/)* est un site-ressource qui donne les informations actuelles sur le support des divers modules CSS et HTML par les navigateurs. Il permet de vérifier ce que les différents navigateurs et leurs versions sont capables d’afficher ou non.
- Le site *[StatCounter](http://gs.statcounter.com/)* donne des statistiques sur les usages du web: les versions de navigateur en utilisation, les tailles d'écran, etc.
- *[Google Webmaster Tools](https://www.google.com/webmasters/tools/)*: Service Google qui, pour un site donné montrera les erreurs de formatage, les liens cassés, les doublons… Bref, l'état de santé d'un site selon Google.
- *[Google Analytics](https://www.google.com/analytics/)*: un outil de Google qui permet de collecter des données d’utilisation pour un site (temps de visite, fréquence des visites, actions effectuées…)
- *[Piwik](https://piwik.org/)*: semblable à Google Analytics, mais c'est un logiciel Open Source. Permet de mieux respecter les données privées des utilisateurs.
- *[Mixpanel](https://mixpanel.com/)*: permet d'analyser de manière très précise les actions effectuées par les visiteurs d'un site.

Pour plus d'informations sur ces outils, lire: *[Tools That Help Inform Design Decisions](http://www.leemunroe.com/design-tracking-services/)*, par Lee Munroe (2015).

Clients FTP
===

FTP:  Protocole web (File Transfer Protocol) permettant d’envoyer des données vers le serveur. À noter qu'on préfèrera utiliser la variante sécurisée, SFTP (crypte les données transmises, et offre une meilleure sécurité sur des réseaux publics).

**[Cyberduck](https://cyberduck.io/):** Excellent gestionnaire FTP, gratuit et open-source, permettant de naviguer sur le serveur distant de son site, créer des signets, éditer des fichiers directement sur le serveur

D'autres clients FTP existent, mais ils partagent généralement les mêmes fonctionalités: [Interarchy](https://nolobe.com/interarchy/), [Transmit](https://panic.com/transmit/), [ForkLift](http://www.binarynights.com/forklift/)...

À noter que certains éditeurs de code permettent de synchroniser directement les fichiers au moment de la sauvegarde.

Prototypage, maquettage, wireframing
===

Les outils graphiques utilisés pour créer des maquettes de sites web sont aujourd'hui très variés. Ces outils sont souvent utilisés aussi bien pour les maquettes de sites que d'applications, ces deux domaines étant confrontés aux mêmes problématiques (multiplicité des écrans et méthodes d'interaction). 

Depuis quelques années, la pertinence des outils de design classiques dans l'environnement du web fait l'objet de vifs débats: 

- Article de Brad Frost: “[The Post-PSD Era](http://bradfrost.com/blog/post/the-post-psd-era/)” (2013) - "Are we entering the Post-PSD Era of web design?" - L'auteur relève des faiblesses de Photoshop pour la réalisation de maquettes web: supports de taille et résolution variable. Eléments interactifs tels que les liens. 
- Article de Emelyn Baker: “[2014 - The Year of Interaction Design Tools](https://medium.com/@extremelyn/2014-the-year-of-design-tools-3c449d771e62#.542hf0q21)”
- Khoi Vinh, mai 2015: “[The State of Design Tools: An Unscientific Survey](https://www.subtraction.com/2015/05/07/the-state-of-design-tools/)” - L'auteur indique: 

> “Prototyping is the Wild West. Every team we met with uses a variety of prototyping tools, whether Pixate, Marvel, InVision, Flinto or others.”

On peut distinguer différentes classes d'outil, répondant à ces modes de travail multiples, et dans une certaine mesure à différentes étapes du processus de création:

- Outils classiques de graphisme (*Photoshop, Illustrator, InDesign, Keynote, Powerpoint*...)
- Outils de wireframing: *UXPin, Balsamiq, Axure, Proto.io* ...
- Outils de design d'interface: *Sketch* ...
- Outils de prototypage: *Just in Mind, Axure, Origami, Pixate* ...
- Outils d'animation: *After Effects, Principle, Framer* ...

#### Outils de Wireframing

*UXPin*, *Balsamiq*, *Axure*, *Proto.io* 

Ces outils servent à produire des "wireframes", càd des représentatons centrées sur la navigation et la répartition de blocs de contenus, sans interférer avec le design graphique. Il est possible de faire cela avec un outil de dessin vectoriel (Illustrator...), mais il existe des outils spécifiquement dédiés. Il est aussi courant de produire des wireframes sur papier.

#### Outils de prototypage

*Axure*, *Just in Mind*, *Pixate*...

À la différence des "wireframes", ces outils servent à produire des maquettes visuelles proches de l'expérience finale, l'écriture de code en moins. On distingue le prototype de la maquette (*mockup*, créé dans un outil comme Photoshop): le prototype vise à simuler non seulement le graphisme, mais aussi le comportement du produit final. Un outil de prototypage permettra de définir les *interactions* et les *transitions* entre les différents écrans du site (ou de l'application).

Certains outils proposent d'inclure tout cela dans une application.

Une autre approche consiste à créer les visuels dans un outil de design (Photoshop, Illustrator, Sketch...), puis de définir les interactions et construire un prototype avec des outils comme *InVision* ou *Marvel* (voir ci-dessous).

<h4>Outils de dessin vectoriel orientés design d'interfaces</h4>

*Sketch*, publié en 2010 par Bohemian Software, est une application de design d’interface très populaire actuellement. Sketch est développé uniquement pour Mac OSX, par une petite équipe de développement basée aux Pays-Bas. Bohemian Software propose également une application pour iOS, *Sketch Mirror*, visant à prévisualiser les créations sur iPhone ou iPad.

La situation des outils de design d'interface est assez particulière: Adobe a stoppé en 2010 le développement de *Fireworks*, utilisé par de nombreux webdesigners pour la création de visuels. En 2011, Adobe lance la suite de logiciels Edge (*Edge Animate, Edge Inspect, Edge Reflow, Edge Code*), afin de s'adapter aux besoins des webdesigners (lire à ce sujet l'article de Aaron Shekey, https://www.aaronshekey.com/work/adobe/). La suite Edge est stoppée en 2015, certains développements étant intégrés dans *Dreamweaver* et *Muse*. En 2016, Adobe dévoile un nouveau logiciel: *Adobe Experience Design* (Adobe XD). C'est visiblement une tentative de contrer le succès de Sketch, et l'accueil des designers UX est [plutôt](http://outsmartlabs.com/blog/sketch-v-s-adobe-xd/) [critique](http://scottjensen.design/2016/04/what-i-think-of-adobe-xd/)...

#### Outils de présentation et communication

Ces outils permettent de construire une maquette interactive avec simulation de navigation, en combinant des images et en définissant des zones cliquables qui permettent de naviguer d'un écran à l'autre. Le travail de design se fait dans une autre application, p.ex. *Photoshop*, *Illustrator* ou *Sketch*. Les fichiers graphiques sont synchronisés, afin de permettre un processus de travail fluide. Ces outils facilitent également la collaboration et la discussion, via leurs fonctions de commentaires et annotations. 

**InVision** - InVision est une entreprise basée à New York. "Launched in 2011, the company has since raised around $80M in four fundraising rounds."
En novembre 2014, InVision annonce [le support du format Sketch](http://blog.invisionapp.com/sketch-meet-rapid-hi-fi-prototyping/).

> "*Marvel* and *InVision* can be compared, but comparing them to *Just in Mind* is just wrong, this is a complete prototyping tool, the other 2 are just for finalization and collaboration." (un internaute)

**Marvel** - Marvel est lancé en 2013 par une startup basée à Londres, comptant en 2016 une vingtaine d'employés. Construit initialement autour de DropBox, Marvel ajoute en 2015 le support des fichiers Sketch.

**Particularités:**

Ces deux applications permettent la synchronisation d'images (PNG ou JPEG) depuis DropBox (ou GoogleDrive).

Les deux applications proposent également un excellent support pour les fichiers **Sketch**:

- *Marvel* propose un plugin pour Sketch, qui permet de synchroniser des *artboards* depuis l'application.
- *InVision* peut synchroniser les fichiers Sketch depuis DropBox, et va créer un écran pour chaque *artboard*.

Tous deux proposent des **applications mobiles**:

- *InVision* propose une application iOS pour iPhone et iPad ([InVision Viewer](https://itunes.apple.com/ch/app/invision-viewer/id990700027?mt=8)), qui permet de naviguer dans les projets, et de les consulter hors-ligne.
- *Marvel* propose une [application iOS](https://itunes.apple.com/ch/app/marvel-design-apps-on-your/id765801658?mt=8) ainsi qu'une [application Android](https://play.google.com/store/apps/details?id=com.marvelapp&hl=en), qui permettent non seulement de visionner les projets (même hors-ligne) mais aussi de [créer et modifier des prototypes](https://blog.marvelapp.com/marvel-for-ios-the-prototyping-tool-for-the-mobile-generation/).

#### Autres approches du Prototypage:

Applications de prototypage utilisant un principe de "patches" (*node based design*):

- *[Origami](https://facebook.github.io/origami/)* - outil développé par Facebook, utilise QuartzComposer, permet de visualiser sur iOs (avec une application, *Origami Live*).
- *[Avocado](https://github.com/ideo/avocado/)* - "an open source interaction design toolbox, built on top of Facebook's Origami framework".

Autre logiciel atypique: *[Framer](https://framerjs.com/)*

La profession du design web étant en rapide évolution, le marché des outils informatiques est particulièrement instable. Les nouveaux outils sont souvent lancés en mode "startup", avec un financement initial modeste et un modèle économique flou. Par conséquent, il n'est pas rare que ces entreprises disparaissent, en se faisant racheter par l'un des "géants": 

**Pixelapse** (2011)
 Permet de comparer visuellement des changements de design pour un site.
 Racheté par Dropbox

**Form** 
- Form était un outil de prototypage créé par une startup de 6 personnes, RelativeWave.
- Achat par Google en 2014.

**Pixate** (2012)
- Slogan: “the most powerful prototyping platform”
- [Campagne Kickstarter](https://www.kickstarter.com/projects/pixate/beautiful-native-mobile-apps/description) en 2012 qui a levé $61,274.
- Achat par Google en 2015. Annonce la fin du développement en 2016.
- En 2016, Google annonce une nouvelle application, *Stage*: "Stage is being brought to you by the teams behind Pixate and Form."

**Macaw** (2014)
- Slogan: “the code-savvy Web design tool”  
- Campagne Kickstarter en 2013 qui a levé $275,929.
- Achat par InVision en 2016, le développement s'achève.

Gestion de projet / collaboration
===

- DropBox : partage de fichiers.
- GoogleDrive : partage de fichiers et création de documents (comparables à Word ou Excel).
- Evernote : permet de créer des carnets de notes partagés.
- Trello : permet de constituer des listes de tâches.
- Basecamp : permet de communiquer et partager des fichiers.
- Etherpad : léger et facile d’utilisation, bloc-notes en ligne, sans login.


Versionnement de code
===

Le versionnement permet de garder et de remonter à des versions antérieures d’un projet, et même de fusionner des changements apportés par plusieurs collaborateurs sur un même fichiers.

Versionnement avec Git
- GitHub app
- SourceTree

## Sécurité

- Services de backup automatique

Backups
===

- Time Machine
- Crashplan :  permet de faire des backups réguliers de certains dossiers importants. Prix de 50$ par année, espace de stockage illimité.

Gestionnaire de mots de passe

- LastPass
- Dashlane
- 1Password
- RoboForm
- Keeper

Ces services offrent des applications desktop et des extensions de navigateur.

Lire: [http://www.panoptinet.com/cybersecurite-decryptee/test-dashlane-lastpass-keepass-quel-logiciel-choisir/](http://www.panoptinet.com/cybersecurite-decryptee/test-dashlane-lastpass-keepass-quel-logiciel-choisir/)

Facturation & mesure du temps
===

Ces outils permettent la visualisation du temps passé à un projet, de faciliter la facturation de ses horaires.

- Freshbooks
- Harvest

Mail, contacts, agenda
===

Clients email:

- Mail, par Apple
- [Thunderbird](https://www.mozilla.org/fr/thunderbird/)
- [Airmail](http://airmailapp.com/) - 10$
- [Postbox](https://www.postbox-inc.com/)

Gestion d'agenda

Gestion de contacts