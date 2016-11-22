---
layout: page
title: Git et Github
permalink: /divers/git/
---

Explication concernant le système de versionnement Git.

**Git** est un logiciel de *gestion de versions* décentralisé, créé en 2005 par Linus Torvalds. C'est un logiciel libre, sous licence GPL. Le site officiel de documentation est [git-scm.com](https://git-scm.com).

GitHub est un service web offrant l'hébergement de projets utilisant Git, lancé en 2008. Devenu extrêmement populaire, GitHub offre de nombreux de communication et la collaboration. 

![](/cours-divers/img/Strip-Bon-daccord-650-final.jpg)

Guide d'utilisation:

- créer un compte.

- télécharger l'application Github Desktop.

- créer un repository.

- synchroniser ses modifications

- remommer la branche "master" en "gh-pages".

- faire un correctif sur un projet existant.

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
- *[Les bases de Git](https://git-scm.com/book/fr/v1/Les-bases-de-Git)*, dans la documentation officielle.

**En anglais:**

*GitHub for the Rest of Us*, par Morten Rand-Hendriksen:  

- [Vidéo de 10 minutes](https://wordpress.tv/2015/12/13/morten-rand-hendriksen-github-for-the-rest-of-us/)
- [Slides](https://mor10.com/github-wcus/)

Logiciels:
===

- [GitHub Desktop](https://desktop.github.com/), client Git (Mac et Windows) développé par GitHub.
- [SourceTree](https://www.sourcetreeapp.com/), client Git (Mac et Windows) développé par Atlassian (société proposant le service BitBucket).
