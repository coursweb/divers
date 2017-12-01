---
layout: page
title: Newsletters
permalink: /divers/newsletters/
---

# Mailing-listes et newsletters

Les Mailing-listes, listes de discussion

Ce sont des outils visant à donner un espace de discussion, une communication entre plusieurs participants.

Outils classiques: Majordomo, Mailman, Sympa...   

Nouveaux outils: [Lurk](http://lurk.org/), [Slack](https://slack.com)

## Les newsletters

Une newsletter est un service de communication "à sens unique", permettant de transmettre de l'information à des abonnés ayant souscrit à la newsletter.

Quelques services de création et d'envoi de newsletters, parmi les plus connus: 

* [MailChimp](https://mailchimp.com/)
* [Tinyletter](https://tinyletter.com/)
* [Mailjet](https://www.mailjet.com/)
* [Constant Contact](https://www.constantcontact.com/)
* [Aweber](https://www.aweber.com/)

Ces services offrent des interfaces web pour composer visuellement une newsletter, pour gérer les abonnés, et pour effectuer les envois.

![Interface de MailChimp](/cours-divers/img/mailchimp-interface.png)

Un produit un peu à part: [Sendy](https://sendy.co/). C'est une application hébergée sur votre serveur, permettant de gérer des newsletters. Les envois se font via le service Amazon SES (ci-dessous), plus économique que les autres systèmes.

## Services d'envoi SMTP

Ce sont des plate-formes d'expédition pour l'envoi d'emails en grande quantité:

* [SendGrid](https://sendgrid.com/)
* [Amazon SES](https://aws.amazon.com/fr/ses/)
* [Mailgun](https://www.mailgun.com/), "The Email Service For Developers"
* Elastic Email

Les différences de prix sont très variables d'un service à l'autre - la gamme va de 0.10$ à 10$ pour l'envoi de 1000 emails.

![Prix d'envoi de 1000 emails (état en 2011)](/cours-divers/img/email-send-price.png)

## Outils de test

[Litmus](http://litmus.com/email-testing) - outil de test pour vérifier le rendu d'une newsletter dans un grand nombre de clients email.

## Délivrabilité

Méthodes d'authentification permettant d'améliorer le taux de délivrabilité d'un domaine email:

- SPF, un système de validation.
- DKIM, un système de signature des messages.


## Ressources

* [Email Design Guide](https://mailchimp.com/email-design-guide/), par Mailchimp