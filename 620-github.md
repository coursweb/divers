---
layout: page
title: Git et GitHub
permalink: /divers/git/
---

Explication concernant le système de versionnement Git.

**Git** est un logiciel de *gestion de versions* décentralisé, créé en 2005 par Linus Torvalds (le créateur de Linux). C'est un logiciel libre, sous licence GPL. Le site officiel de documentation est [git-scm.com](https://git-scm.com).

**GitHub** est un service web offrant l'hébergement de projets utilisant Git, lancé en 2008 (cf. [cet article](http://tom.preston-werner.com/2011/03/29/ten-lessons-from-githubs-first-year.html) sur les débuts de cette startup californienne). Devenu extrêmement populaire, GitHub offre de nombreuses fonctionnalités facilitant la communication et la collaboration. 

Quelques services d'hébergement Git: 

* [GitHub](https://github.com/), le plus utilisé avec plus de 14 millions d'utilisateurs (état 2016). 
* [BitBucket](https://bitbucket.org), un service freemium, acquis par la société australienne Atlassian en 2010.
* [GitLab](https://about.gitlab.com/gitlab-com/), à la fois un service en ligne comparable à GitHub, et un outil serveur open-source.
* [Framagit](https://framagit.org), un service reposant sur Gitlab, maintenu par l'association Framasoft.

![publication marketing de GitHub](/cours-divers/img/github-activity-book.jpg)

Terminologie Git
==

**Commit** (commettre) : Valider vos modifications (a snapshot of your repo)

**Push** (pousser) : send commits to a remote

**Pull** (tirer) : get commits from a remote

**Checkout** : time travel to a specific commit

**Stash** (ranger) : save modified and staged changes (en français: remise)

**Merge** (fusionner) : combining two branches

**Rebase** (rembobiner) : apply any commits of current branch ahead of specified one

**Branch** (branche) : create a new branch at the current commit (a movable label that points to a commit)

**index** : aussi "stage", "staging area": Il s’agit de la zone de validation désignant les travaux que vous souhaitez voir apparaître dans votre prochain commit.

**HEAD** : HEAD est un pointeur, une référence sur notre position actuelle dans notre répertoire de travail Git. "The current HEAD is local to each repository, and is therefore individual for each developer."

![](/cours-divers/img/Strip-Bon-daccord-650-final.jpg)

Guide d'utilisation GitHub:
==

(Documentation à compléter)

- créer un compte.
- Télécharger l'application [Github Desktop](https://desktop.github.com/).
- Créer un repository.
- Synchroniser ses modifications
- Remommer la branche "master" en "gh-pages".
- Faire un correctif sur un projet existant.

Utiliser Github Pages:
==

Comment créer un site hébergé dans Github Pages:

<h3>Réglages à faire dans l'administration DNS de votre hébergeur</h3>

- Réfléchissez au type de domaine que vous souhaitez utiliser. 
- Rendez-vous dans la gestion des zones DNS de votre domaine (chez Infomaniak ou autre).
- Pour trouver cet endroit chez Infomaniak, connectez-vous à [admin2.infomaniak.com](https://admin2.infomaniak.com/), allez dans : *Nom de domaine > Nom de votre domaine > Gestion des DNS*, puis cliquez le bouton "Gérer les zones DNS".

**Option sous-domaine:**

- Si le domaine comporte un sous-domaine, comme portfolio.example.com, ou www.example.com, vous devrez créer une entrée de type CNAME.
- Renseignez "Champ/Field" (entrer le sous-domaine choisi), et "Cible/Target" (username.github.io). Si votre utilisateur est p.ex. Gandalf69, vous entrerez : gandalf69.github.io (tout en minuscules).
- Vous pouvez laisser le champ TTL avec sa valeur par défaut.

![Ajout de CNAME chez Infomaniak](/cours-divers/img/github-dns-cname.png)

![Ajout de CNAME chez O2Switch](/cours-divers/img/git-cname-o2switch.png)

**Option "apex domain":**

- Si le domaine est dépourvu de sous-domaine, comme **cours-web.ch** (un "apex domain"), la procédure est différente. Il faudra créer deux entrées de type A.
- Renseignez "Cible" et entrez les adresses IP fournies par Github dans leur documentation, à savoir 192.30.252.153 et 192.30.252.154 (une pour chaque entrée A).
- Vous pouvez laisser le champ TTL avec sa valeur par défaut.

![Ajout de zone A chez Infomaniak](/cours-divers/img/git-apex-infomaniak.png)

![Même réglage, chez Hostpoint](/cours-divers/img/git-apex-hostpoint.png)

<h3>Réglages à faire dans GitHub</h3>

- Premièrement, votre projet doit être publié sur GitHub.
- Créer une nouvelle branche, que vous nommez "gh-pages".
- Si vous n'utilisez pas la branche "master", vous pouvez définir "gh-page" comme branche principale (et effacer la branche "master" pour éviter les confusions).
- Aller dans les "Settings" de votre projet, dans la partie "Github Pages"
- Renseignez le domaine, p.ex. portfolio.example.com
- Enregistrez ("Save") - ça y est, votre site fonctionne!

![Saisie du domaine pour GitHub Pages](/cours-divers/img/github-custom-pages.png)

Références GitHub: 

* [Using a custom domain with GitHub Pages](https://help.github.com/articles/using-a-custom-domain-with-github-pages/)
* [About supported custom domains](https://help.github.com/articles/about-supported-custom-domains/)
* [Setting up an apex domain](https://help.github.com/articles/setting-up-an-apex-domain-and-www-subdomain/)


Ecriture de messages de Commit
===

"En règle générale, les messages doivent débuter par une ligne unique d’au plus 50 caractères décrivant concisément la modification, suivie d’une ligne vide, suivie d’une explication plus détaillée. Le projet Git exige que l’explication détaillée inclue la motivation de la modification en contrastant le nouveau comportement par rapport à l’ancien — c’est une bonne règle de rédaction."

Source: [The Git Book](https://git-scm.com/book/fr/v2/Git-distribu%C3%A9-Contribution-%C3%A0-un-projet)

![Messages de Commit](/cours-divers/img/git-commit-messages.png)

Source: *Git for Humans*, présentation par Alice Bartlett, développeuse au Financial Times

Les branches
===

Un explicatif des branches dans l'interface SourceTree: [Use SourceTree branches to merge an update](https://confluence.atlassian.com/bitbucket/use-sourcetree-branches-to-merge-an-update-732268925.html)

Un workflow Git
===

Une méthodologie Git pour projets de design, proposée par [Mathieu Dutour](https://mathieudutour.github.io/git-sketch-plugin/), auteur du *Git Sketch Plugin*:

* Créez une nouvelle *branche* quand vous commencez à travailler sur une nouvelle fonctionalité.
* Travaillez normalement sur votre design.
* Enregistrez le fichier.
* Faites un "Commit" de vos modifications, avec un message les décrivant.
* Faites un "Push" de vos modifications.
* Faites une "pull request" de votre branche vers la branche principale ("master").
* Voilà! Vos collaborateurs peuvent voir vos modifications, faire des commentaires, et les approuver. Une fois approuvés, faire un "merge" de votre "pull request".

<h3>Liens sur les workflows Git:</h3>

* [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/), article de Vincent Driessen, 2010, définissant la méthodologie "Git Flow". Propose un système de branches.
* [Using git-flow to automate your git branching workflow](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/), par Jeff Kreeftmeijer - donne des informations techniques sur la manière d'appliquer le modèle "Git Flow" (et l'utilitaire [git-flow](https://github.com/nvie/gitflow), qui est "a wrapper around existing git commands").
* [GitHub Flow](http://scottchacon.com/2011/08/31/github-flow.html), article de  Scott Chacon, 2011, qui décrit une méthode plus simple et fluide (pratiquée par l'entreprise GitHub, d'où son nom).
* [A simple git branching model](https://gist.github.com/jbenet/ee6c9ac48068889b0912), par Juan Benet, 2013.
* [Simple Git workflow is simple](http://blogs.atlassian.com/2014/01/simple-git-workflow-simple/), article de Nicola Paolucci, 2014.
* [GitLab Flow](https://about.gitlab.com/2014/09/29/gitlab-flow/), article de Sytse Sijbrandij, 2014 - une méthode qui vise à prévenir la complexité de Git Flow: "git flow is too complex for most of the use cases".
* [Comparing Workflows](https://www.atlassian.com/git/tutorials/comparing-workflows), documentation d'Atlassian (la société produisant Bitbucket et Sourcetree)

Quelques autres articles sur l'utilisation de Git:

- [Bien utiliser Git merge et rebase](http://www.git-attitude.fr/2014/05/04/bien-utiliser-git-merge-et-rebase/), par Christophe Porteneuve (git-attitude), 2014

Difficile?
===

Git n'est certainement pas un outil simple. Voici quelques citations qui le confirment:

> Git isn’t difficult because you’re not smart enough, or because you missed an important meeting. Git is difficult because Git is difficult.

David Demaree, auteur de *Git for Humans*

> I’m not good with Git, and still don’t fully understand how rebasing works. I messed up my commits a couple of times. Not a big deal, but I got different error messages no matter which workflow I tried. I realized that I need to know more about Git, and be more patient.

Sami Keijonen, développeur, [dans un article](https://poststatus.com/contributing-to-twenty-seventeen-theme/) où il relate sa contribution au thème WordPress TwentySeven.

Il est important de réaliser que le plus important, avec Git, c'est d'adopter la pratique du "versionnement" dans son processus de travail. Ce n'est pas seulement un outil, un logiciel - c'est un ensemble de méthodes pour mieux organiser le travail collaboratif.

Troubleshooting
===

**Problème:** Lors de la synchronisation, Git dit: *Sync Failed - There are both local and remote commits. Please commit all your changes and then sync again*.

**Tentative:** 

- Cocher toutes les modifications ("Uncommited changes").
- Faire un "Commit".
- Refaire un "Sync". Message : *Sync Conflicts: Please resolve all conflicted files, commit, then try syncing again*.
- Faire un click-droit sur les fichiers affichés, faire "Discard Changes"...

**Résultat:**  

Le résultat n'est pas celui escompté...

```
error: failed to push some refs to 'https://github.com/monprojet.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

**Solution:** 

- Comme le dit l'explicatif, il faut intégrer tout d'abord les modifications du serveur (avec un pull).
- Si des "Merge conflicts" apparaissent... les résoudre.

***

**Problème:**  
On se trouve avec des modifications non voulues. Comment revenir d'une version en arrière?

**Solution:**  
Se rendre dans l'historique de Github Desktop, et retourner dans une version antérieure avec un double click.

***

**Problème:** on a des caractères étranges dans un document, comme ceci: 

```
<<<<<<< HEAD
    Une version de mon projet
=======
    Une autre version de mon projet
>>>>>>> master
```

**Solution:** Ces symboles sont des délimiteurs nommés "conflict markers", ils indiquent un conflit non-résolu entre deux versions d'un même fichier, que Git n'a pas pu résoudre automatiquement.

Vous devez les corriger soit en effaçant l'une des versions, soit en utilisant une fonction "Resolve a Merge" dans votre logiciel Git.

***

Pour sa présentation *"[Changing History, or How to Git pretty](http://justinhileman.info/article/changing-history/)"*, Justin Hileman a créé le graphe "escape a git mess, step-by-step" - visuel qui explique les différentes manières de résoudre des problèmes dans Git:

![escape a git mess, step-by-step](/cours-divers/img/git-pretty.png)

Documentation:
===

- *[GitHub Pour les Nuls](http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/)*, par Lauren Orsini, trad. Christophe Ducamp, 2013.
- *[Gérez vos codes source avec Git](https://openclassrooms.com/courses/gerez-vos-codes-source-avec-git)*, un cours sur OpenClassroooms, par Mathieu Nebra.
- *[Les bases de Git](https://git-scm.com/book/fr/v12)*, dans la documentation officielle de Git.
- [git-guide](http://rogerdudler.github.io/git-guide/index.fr.html), par Roger Dudler (traduit par KokaKiwi)
- [intro-git](http://liris.cnrs.fr/~pchampin/enseignement/intro-git/), support réalisé par Pierre-Antoine Champin et Amélie Cordier
- [Git Cheatsheet](http://ndpsoftware.com/git-cheatsheet.html), par Andrew Peterson

**En anglais:**

- *[Git from the Bottom Up](https://jwiegley.github.io/git-from-the-bottom-up/)*, par John Wiegley
- *GitHub for the Rest of Us* (explication de Git par la science-fiction), par Morten Rand-Hendriksen: [Vidéo de 10 minutes](https://wordpress.tv/2015/12/13/morten-rand-hendriksen-github-for-the-rest-of-us/) / [Slides](https://mor10.com/github-wcus/)
- *[Think Like (a) Git](http://think-like-a-git.net/)*, une explication par Sam Livingston-Gray, 2011.
- *[Get Started with Git](http://alistapart.com/article/get-started-with-git)*, par Al Shaw, A List Apart #317, 2010. 
- *[Git: The Safety Net for Your Projects](http://alistapart.com/article/git-the-safety-net-for-your-projects)*, par Tobias Günther, A List Apart #402, 2014

Logiciels:
===

Quelques clients Git qui proposent une interface graphique, en alternative à la ligne de commande:

- [GitHub Desktop](https://desktop.github.com/), client Git (Mac et Windows) développé par GitHub.
- [SourceTree](https://www.sourcetreeapp.com/), client Git (Mac et Windows) développé par Atlassian (société proposant le service BitBucket).
- [GitKraken](https://www.gitkraken.com/), "Free for open source, education, non‑profit, startups or personal use".
- [SmartGit](http://www.syntevo.com/smartgit/ ), "can be used free of charge by Open Source developers, teachers and their students, or for hobby, non-paid usage."

Un utilitaire ligne de commande, pour utiliser des commandes en français:

- https://gist.github.com/remiprev/1110021