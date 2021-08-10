---
layout: page
title: La syntaxe MarkDown
permalink: markdown.html
---

MarkDown est un petit projet lancé en 2004 par le bloggeur [John Gruber](https://fr.wikipedia.org/wiki/John_Gruber). C'est une syntaxe minimale permettant d'écrire du texte pour le web, puis de le convertir en HTML.

Elle a été adoptée par des sites comme StackOverflow, Github (pour la rédaction de commentaires, ou dans le README). Depuis 2016, WordPress.com permet d'écrire en MarkDown.

## gras, italique, souligné

Pour obtenir du **gras**: entourer le texte de \*\*deux astériques\*\*.

    *italic*   **bold**
    _italic_   __bold__

## titres et séparateurs

```
Header 1
========

Header 2
--------

# Header 1 #

## Header 2 ##

###### Header 6
```

## Liens et images

```
An [example](http://url.com/ "Title")

An [example][id]. Then, anywhere
else in the doc, define the link:

[id]: http://example.com/  "Title"

![alt text](/path/img.jpg "Title")

![alt text][id]

[id]: /url/to/img.jpg "Title"
```

## Listes

## Blocs de code

Retours de ligne: 

```
Roses are red,   
Violets are blue.
```

Lignes horizontales: 

```
---

* * *

- - - - 
```

Blocs de citation:

```
> Email-style angle brackets
> are used for blockquotes.

> > And, they can be nested.

> #### Headers in blockquotes
> 
> * You can quote a list.
> * Etc.
```

## Ressources

Editeurs de texte conçu pour le MarkDown: 

* *[ByWord](https://bywordapp.com/)*
* *[iA Writer](https://ia.net/writer/)*
* *[MacDown](https://macdown.uranusjr.com/)* (gratuit et open-source)
* [Typora](https://typora.io/)
* [Mark Text](https://marktext.app/)

Un éditeur de text affichant d'un côté le code MarkDown, de l'autre le résultat produit:

![Edition MarkDown](img/mou-editor.png)

Vous avez aussi un très bon support dans ces éditeurs de code: 

* *Atom*
* *Visual Studio Code*

* [Article Wikipédia](https://fr.wikipedia.org/wiki/Markdown)
* [définition de la syntaxe MarkDown](https://daringfireball.net/projects/markdown/syntax) par John Gruber
* [Un tutoriel sur OpenClassrooms](https://openclassrooms.com/courses/redigez-en-markdown)
* [MarkDown Quick Reference](http://en.support.wordpress.com/markdown-quick-reference/) (anglais)

### Approfondissement

- Mpondo-Dicka Patrick, « [Le Markdown, une praxis énonciative du numérique](http://dx.doi.org/10.25965/interfaces-numeriques.3915) », *Interfaces numériques*, 2019, vol. 8, n°2.
