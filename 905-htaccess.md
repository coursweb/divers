---
layout: page
title: htaccess
permalink: /divers/htaccess/
---

Explication concernant le fichier `.htaccess`.

Ce fichier, placé dans le dossier racine d'un site tournant sur un serveur Apache, permet d'effectuer un certain nombre de réglages: 

- Optimisation de vitesse (compression gzip)
- Durée du cache: mise en cache avec une durée spécifiée par format.
- Forcer des redirections.
- Empêcher l'accès à certains contenus.

Une bonne référence: le HTML5 Boilerplate donne de nombreux conseils d'optimisation de vitesse.

[https://github.com/h5bp/html5-boilerplate/blob/master/dist/.htaccess](https://github.com/h5bp/html5-boilerplate/blob/master/dist/.htaccess)

## Autoriser le chargement de webfont depuis un autre domaine

Certains navigateurs vont refuser de charger une ressource qui est hébergée sur un domaine différent du HTML actuel.

Pourtant cela peut être nécessaire, par exemple dans le cas d'un blog Tumblr pour lequel vous aimeriez utiliser une webfont depuis votre propre domaine.

Pour autoriser cela, vous devez ajouter un réglage HTACCESS au domaine qui héberge la fonte:

```
<IfModule mod_headers.c>
   Header set Access-Control-Allow-Origin "*"
</IfModule>
```

## Empêcher l'accès à des contenus

Ce cas de figure se présente notamment pour l'utilisation de **webfonts** commerciales. Certaines fonderies - p.ex. [Lineto](https://lineto.com/), ou [Fatype](https://fatype.com/) - demandent de protéger les fontes par une restriction .htaccess.

L'idée est de permettre le chargement uniquement depuis un nom de domaine précis: si la fonte est chargée via une feuille de style CSS depuis le domaine example.com, elle sera disponible. Toutes les autres demandes d'accès à la fonte seront refusées - il est donc impossible de télécharger les fichiers. 

Voici un exemple de code .htaccess qui produit cet effet:

```
<FilesMatch "\.(eot|woff|svg|ttf)$">
    RewriteEngine On

    # Let proxy servers with empty referer through
    
    RewriteCond %{HTTP_REFERER}             ^$
    RewriteCond %{HTTP:VIA}                 !^$ [OR]
    RewriteCond %{HTTP:USERAGENT_VIA}       !^$ [OR]
    RewriteCond %{HTTP:FORWARDED}           !^$ [OR]
    RewriteCond %{HTTP:FORWARDED-FOR}       !^$ [OR]
    RewriteCond %{HTTP:X-FORWARDED}         !^$ [OR]
    RewriteCond %{HTTP:X-FORWARDED-FOR}     !^$ [OR]
    RewriteCond %{HTTP:X_FORWARDED_FOR}     !^$ [OR]
    RewriteCond %{HTTP:PROXY_CONNECTION}    !^$ [OR]
    RewriteCond %{HTTP:XPROXY_CONNECTION}   !^$ [OR]
    RewriteCond %{HTTP:HTTP_PC_REMOTE_ADDR} !^$ [OR]
    RewriteCond %{HTTP:HTTP_CLIENT_IP}      !^$
    RewriteRule .* - [PT,L]

    # For everybody else, the referer must match the domains for which this
    # web-font is licensed.
    
    RewriteCond %{HTTP_REFERER} !:\/\/([^.]+\.|)exemple.com
    RewriteRule .* - [F]

    # Set Cache-Control header to must-revalidate, as we want clients to check
    # against the above rules on each request.
    Header set Cache-Control "must-revalidate"
    
</FilesMatch>
```