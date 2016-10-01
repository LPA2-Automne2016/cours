# Les exemples

On l'a dit tout à l'heure un webservice permet de communiquer au travers d'une API avec une application.

Communiquer ? Mais pour quoi faire ?

<img src="http://bernard.tribollet.pagesperso-orange.fr/SiteRegionR-A/Rubriques/EssaiErreurShadok/PasdePb.jpg" border="0" height="400" width="278">

## Qu'est-ce qu'une [API](https://en.wikipedia.org/wiki/Application_programming_interface)

*An API (**A**pplication **P**rogramming **I**nterface) is  a set of functions and procedures that allow the creation of applications which access the features or data of an operating system, application, or other service.*

Une API est en quelque sorte un contrat que l'application passe avec les personnes de l'extérieur qui voudraient utiliser les services de l'application. Par nécessité, elle doit être documentée et stable.

**ATTENTION** API ne veut pas systématiquement dire webservice ! Ne pas confondre. Dans la suite de nos travaux, les API seront très souvent utilisées au travers d'un webservice.

## Quelques cas d'usage
Dans le cadre du devoir de cette semaine, nous venons de mettre en place une intégration entre github et travis. Sans le savoir, vous venez de mettre en mouvement un certain nombre de communications entre les différents éléments du projet.

* **Comment travis-CI sait-il que github vient d'enregistrer un commit ?**
    * Car Github sur réception d'un push va utiliser l'API/webservice de travis pour lui demander de déclencher un build : https://docs.travis-ci.com/user/triggering-builds

* **Comment travis-CI fait-il pour déployer vers heroku ?**
    * via l'API de heroku https://devcenter.heroku.com/categories/platform-api

* **Comment Slack fait-il pour recevoir les notifications lorsque quelqu'un modifie github ?**
    * A votre avis ?

## Pour un développeur les API/webservices servent à quoi ?
![reponse de norman](http://www.etaletaculture.fr/wp-content/uploads/2015/12/une-reponse-de-normands.jpg)

Tout va dépendre de l'application que l'on développe et des demandes des utilisateurs. De nos jours, il y a des webservices pour tout !
Une des tendances lourde du marché concerne les réseaux sociaux. Quasi tout le monde veut/doit être présent sur les réseaux sociaux :
* https://developers.facebook.com/
* https://dev.twitter.com/rest/public
* https://developers.google.com/+/domains/api/circles

Il existe aussi tout un monde plus lié au métier de l'informatique, ces webservices vont par exemple offrir des services aux développeurs pour leur permettre de déployer plus facilement leur application, exemple: Travis/github/heroku

Suite : [le fonctionnement](./03-fonctionnement.md)