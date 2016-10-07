---
layout: page
title: Outils de développement web
permalink: /divers/outils/
---

> "Tools are dangerous - they can give you the illusion of knowing what you're doing." @p3ob7o at #wcch

Cet article présente une liste d'outils et logiciels utiles pour le design et la programmation web. 

Editeurs de code:
===

* [TextWrangler](http://www.barebones.com/products/TextWrangler/ 
) - éditeur gratuit 
* [Sublime Text](https://www.sublimetext.com/) - éditeur gratuit, le plus populaire en ce moment. Il existe [un grand nombre d'extensions](https://packagecontrol.io/) pour étendre ses fonctionalités. 
* [Atom](https://atom.io/) - éditeur gratuit et open source, très similaire à Sublime Text. Il existe également [des extensions](https://atom.io/packages).
* [Coda](https://panic.com/coda/) - éditeur avec des fonctions de prévisualisation. Prix: $99.
* [Espresso](http://www.macrabbit.com/espresso/) - éditeur avec des fonctions de prévisualisation du CSS. Prix: $75. Développement en standby depuis juin 2015.
* [PhpStorm](https://www.jetbrains.com/phpstorm/) - éditeur spécialisé pour le langage PHP (utile pour le développement de thèmes WordPress, par exemple).

Parmi les fonctionalités partagées par tous ces éditeurs de code: 

- la colorisation de la syntaxe pour faciliter la lecture et la détection d’erreurs.
- la suggestion de termes propres au langage utilisé (HTML, CSS, JavaScript, etc).
- le  « rechercher remplacer » à l'échelle d'un projet ou dossier.
- le « rechercher remplacer » avec des « expressions régulières ».

**L'inspecteur du navigateur** est un outil indispensable pour le développement d'interfaces web. Il permet l’analyse des éléments de mise en page d’un site, son chargement, son poids etc. Il est disponible dans les navigateurs majeurs (Firefox, Chrome, Safari). À noter que Firefox propose une "[version développeur](https://www.mozilla.org/fr/firefox/developer/)".

Statistiques & outils d'analyse
===

- **[Can I Use](http://caniuse.com/)** est un site-ressource qui donne les informations actuelles sur le support des divers modules CSS et HTML par les navigateurs. Il permet de vérifier ce que les différents navigateurs et leurs versions sont capables d’afficher ou non.
- **Statistiques Web:** le site [StatCounter](http://gs.statcounter.com/) donne des informations sur les usages du web: les versions de navigateur en utilisation, les tailles d'écran, etc.
- **[Google Webmaster Tools](https://www.google.com/webmasters/tools/):** Service Google qui, pour un site donné montrera les erreurs de formatage, les liens cassés, les doublons… Bref, l'état de santé d'un site selon Google.
- **[Google Analytics](https://www.google.com/analytics/):** un outil de Google qui permet de collecter des données d’utilisation pour un site (temps de visite, fréquence des visites, actions effectuées…)
- **[Piwik](https://piwik.org/):** semblable à Google Analytics, mais c'est un logiciel Open Source. Permet de mieux respecter les données privées des utilisateurs.
- **[Mixpanel](https://mixpanel.com/):** permet d'analyser de manière très précise les actions effectuées par les visiteurs d'un site.

Clients FTP
===

FTP:  Protocole web (File Transfer Protocol) permettant d’envoyer des données vers le serveur.

**[Cyberduck](https://cyberduck.io/):** Excellent gestionnaire FTP, gratuit et open-source, permettant de naviguer sur le serveur distant de son site, créer des signets, éditer des fichiers directement sur le serveur

D'autres clients FTP existent, mais ils partagent généralement les mêmes fonctionalités: [Interarchy](https://nolobe.com/interarchy/), [Transmit](https://panic.com/transmit/), [ForkLift](http://www.binarynights.com/forklift/)...

À noter que certains éditeurs de code permettent de synchroniser directement les fichiers au moment de la sauvegarde.

Prototypage, maquettage, wireframing
===

Les outils graphiques utilisés pour créer des maquettes de sites web sont très variés, 

On peut distinguer:

- Les outils classiques de graphisme (Photoshop, Illustrator, InDesign, Keynote, Powerpoint...)
- Des outils de wireframing: UXPin, Balsamiq, Axure, Proto.io 
- Outils d'animation

Débat autour des outils de webdesign: 

- Article de Brad Frost: “[The Post-PSD Era](http://bradfrost.com/blog/post/the-post-psd-era/)” (2013) - "Are we entering the Post-PSD Era of web design?" - L'auteur relève des faiblesses de Photoshop pour la réalisation de maquettes web: supports de taille et résolution variable. Eléments interactifs tels que les liens. 

- Article de Emelyn Baker: “[2014 - The Year of Interaction Design Tools](https://medium.com/@extremelyn/2014-the-year-of-design-tools-3c449d771e62#.542hf0q21)”

- Khoi Vinh, mai 2015: “The State of Design Tools: An Unscientific Survey”

“Prototyping is the Wild West. Every team we met with uses a variety of prototyping tools, whether Pixate, Marvel, InVision, Flinto or others.”

**Outils de Wireframing:**
p.ex.  UXPin, Balsamiq, Axure, Proto.io 

**Outils de prototypage**

Axure, Just in Mind...

**Outils de dessin vectoriel orientés design d'interfaces**

[Sketch](https://www.sketchapp.com/) (2010)
app MacOS de design d’interface très populaire actuellement.
il existe une application pour iOS, *Sketch Mirror*.
L'icône de sketch est venue à symboliser le designer web...

Adobe a stoppé le développement de *Fireworks*, et de la série Edge (*Edge Animate, Edge Inspect, Edge Reflow, Edge Code*). Certains développements seront intégrés dans *Dreamweaver* et *Muse*. En 2016, Adobe dévoile un nouveau logiciel: *Adobe Experience Design*. 

*Affinity Designer* est un outil de dessin vectoriel, concurrent à Adobe Illustrator.

**Outils de présentation et communication**

Ces outils permettent de construire une maquette interactive avec simulation de navigation, en combinant des images produites dans Photoshop ou Sketch. Ils facilitent la collaboration et la discussion (gestion des commentaires et annotations). 

**InVision** - "InVision is a product and prototype design tool used by hundreds of companies including Uber, Twitter, and Airbnb. Launched in 2011, the company has since raised around $80M in four fundraising rounds."

"*Marvel* and *InVision* can be compared, but comparing them to *Just in Mind* is just wrong, this is a complete prototyping tool, the other 2 are just for finalization and collaboration."

Marvel:
"If you've created designs in Sketch, Keynote, Photoshop or powerpoint, you can import these to Marvel to create your prototype."
"You can also import PNG and JPEG images straight from your computer or from Dropbox or Google Drive."

Autres approches du Prototypage

Applications de prototypage utilisant un principe de "patches" (node based design):
- *Origami* - outil développé par Facebook, utilise QuartzComposer, permet de visualiser sur iOs (avec une application, Origami Live).
- *Avocado*

Autre logiciel atypique: *Framer*

Exemples d'outils n'ayant pas survécu à l'instabilité du marché: 

**Pixelapse** (2011)
 permet de comparer visuellement des changements de design pour un site.
 racheté par Dropbox

**Pixate** (2012)
“the most powerful prototyping platform”
- [Campagne Kickstarter](https://www.kickstarter.com/projects/pixate/beautiful-native-mobile-apps/description) en 2012 qui a levé $61,274.
- Achat par Google en 2015. Annonce la fin du développement en 2016.

**Macaw** (2014)
“the code-savvy Web design tool”  
- Campagne Kickstarter en 2013 qui a levé $275,929.
- Acheté par InVision en 2016, le développement s'achève.

Gestion de projet / collaboration
===

- GoogleDrive
- Dropbox
- Evernote 
- Trello
- Basecamp
- Etherpad : léger et facile d’utilisation, interface d’écriture en ligne (bloc note en ligne) sans login


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
- Thunderbird
- Postbox
- Airmail

Gestion d'agenda

Gestion de contacts