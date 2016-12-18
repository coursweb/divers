---
layout: page
title: Git et Github
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

![](/cours-divers/img/Strip-Bon-daccord-650-final.jpg)

Guide d'utilisation:

- créer un compte.

- télécharger l'application Github Desktop.

- créer un repository.

- synchroniser ses modifications

- remommer la branche "master" en "gh-pages".

- faire un correctif sur un projet existant.

Un workflow Git
===

Une méthodologie Git pour projets de design, proposée par [Mathieu Dutour](https://mathieudutour.github.io/git-sketch-plugin/), auteur du Git Sketch Plugin:

* Créez une nouvelle branche quand vous commencez à travailler sur une nouvelle fonctionalité
* Travaillez normalement sur votre design
* Enregistrez le fichier
* Faites un "Commit" de vos modifications, avec un message les décrivant.
* Faites un "Push" de vos modifications.
* Faites une "pull request" de votre branche vers la branche principale ("master").
* Voilà. Vos collaborateurs peuvent voir vos modifications, faire des commentaires, et les approuver. Une fois approuvés, faire un "merge" de votre "pull request".

<h3>Liens sur les workflows Git:</h3>

* [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/), article de Vincent Driessen, 2010, définissant la méthodologie "Git Flow". Propose un système de branches.
* [Using git-flow to automate your git branching workflow](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/), par Jeff Kreeftmeijer - donne des informations techniques sur la manière d'appliquer le modèle "Git Flow" (et l'utilitaire [git-flow](https://github.com/nvie/gitflow), qui est "a wrapper around existing git commands").
* [GitHub Flow](http://scottchacon.com/2011/08/31/github-flow.html), article de  Scott Chacon, 2011, qui décrit une méthode plus simple et fluide (pratiquée par l'entreprise GitHub, d'où son nom).
* [A simple git branching model](https://gist.github.com/jbenet/ee6c9ac48068889b0912), par Juan Benet, 2013.
* [Simple Git workflow is simple](http://blogs.atlassian.com/2014/01/simple-git-workflow-simple/), article de Nicola Paolucci, 2014.
* [GitLab Flow](https://about.gitlab.com/2014/09/29/gitlab-flow/), article de Sytse Sijbrandij, 2014 - une méthode qui vise à prévenir la complexité de Git Flow: "git flow is too complex for most of the use cases".
* [Comparing Workflows](https://www.atlassian.com/git/tutorials/comparing-workflows), documentation d'Atlassian (la société produisant Bitbucket et Sourcetree)

Troubleshooting
===

Lors de la synchronisation, Git dit: "Sync Failed - There are both local and remote commits. Please commit all your changes and then sync again".

Tentative: 
- Cocher toutes les modifications ("Uncommited changes".
- Faire un commit.
- Refaire un sync. Message : "Sync Conflicts: Please resolve all conflicted files, commit, then try syncing again".
- Faire un click-droit sur les fichiers affichés, faire "Discard Changes"...

Résultat: 
- Le résultat n'est pas celui escompté...

error: failed to push some refs to 'https://github.com/think2make/Faire.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Solution: 
- Comme le dit l'explicatif, il faut intégrer tout d'abord les modifications du serveur (avec un pull).
- Si des "Merge conflicts" apparaissent... les résoudre.

Problème: on se trouve avec des modifications non voulues. Comment revenir d'une version en arrière?





Documentation:
===

- *[GitHub Pour les Nuls](http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/)*, par Lauren Orsini, trad. Christophe Ducamp, 2013.
- *[Gérez vos codes source avec Git](https://openclassrooms.com/courses/gerez-vos-codes-source-avec-git)*, un cours sur OpenClassroooms, par Mathieu Nebra.
- *[Les bases de Git](https://git-scm.com/book/fr/v1/Les-bases-de-Git)*, dans la documentation officielle de Git.

**En anglais:**

*GitHub for the Rest of Us*, par Morten Rand-Hendriksen:  

- [Vidéo de 10 minutes](https://wordpress.tv/2015/12/13/morten-rand-hendriksen-github-for-the-rest-of-us/)
- [Slides](https://mor10.com/github-wcus/)

Logiciels:
===

- [GitHub Desktop](https://desktop.github.com/), client Git (Mac et Windows) développé par GitHub.
- [SourceTree](https://www.sourcetreeapp.com/), client Git (Mac et Windows) développé par Atlassian (société proposant le service BitBucket).
