---
layout: page
title: Copier via le terminal
permalink: /divers/copier-terminal/
---

Copier des fichiers via le terminal, cela peut être très utile:

Quand on doit migrer une grande quantité de données, et que le Finder (le système MacOS) n'est pas assez fiable. Quelques insuffisances de la copie par le Finder: 

- si une erreur se produit (p.ex. un fichier étant corrompu), le finder va interrompre la copie.
- une fois un transfer interrompu, il n'est pas possible de le redémarrer à l'endroit où on l'a interrompu.



Avec le terminal, il existe des outils de copie très efficaces. L'un d'entre eux est **rsync**.

Un exemple pour copier un dossier depuis un point d'origine:

```rsync -avP /Dossier/Original /Volumes/DisqueArchive/Copie```

Explicatifs:

* -a is for archive, which preserves ownership, permissions etc.
* -v is for verbose, so I can see what's happening (optional)
* -P or --progress shows progress for each file individually. 

