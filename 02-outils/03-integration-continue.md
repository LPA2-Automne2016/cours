# L'intégration continue
![en essayant continuellement on finit par réussir](http://www.ziserman.com/blog/.images/0803/shadok.jpg)

## Objectif de l'intégration continue
**L'intégration continue (IC) n'a de sens que dans la mesure où le code est testé automatiquement.**
Le dispositif sert de juge de paix : il arrive fréquemment qu'un développement introduise une régression par ailleurs dans le code.
Lors de la remontée du code vers le CVS, l'intégration continue va démarrer et lancer l'intégralité des tests.
Ceci va avoir pour effet de mettre en évidence la régression et de permettre à l'auteur de corriger au plus vite.

En effet, lors de la maturation du projet, la suite de tests devient de plus en plus lourde et il devient trop long pour un développeur de tout lancer. L'intégration continue permet de s'assurer qu'aucun code ne peut parvenir en production sans passer au paravant par la totalité des tests.

Une fois une intégration réalisée, la bonne pratique est de mettre à jour le statut du code directement dans le CVS pour indiquer à tout le monde si le code peut être utilisé et intégré en sécurité.

## Dépendance par rapport aux autres pratiques
On l'a vu auparavant : l'IC ne sert à rien sans suite de test à lancer. 
Par ailleurs, elle permet d'éviter qu'un développeur contourne le système de gestion de dépendance en ajoutant une librairie à la main. 
Si la librairie installée à la main n'est pas déclarée dans le build, l'intégration échouera.
On parle souvent de juge de paix pour désigner l'IC

![la loi c'est moi](http://auto.img.v4.skyrock.net/0326/90540326/pics/3207941217_1_2_CHYSSQfs.png)

Suite : [Le déploiement continu](04-le-deploiement-continu.md)

## Références
Quelques sites permettant d'ajouter l'intégration continue à la gestion de code

* https://travis-ci.org/
* https://codeship.com/
* https://snap-ci.com/
* http://circleci.com/
* 

## Source

*http://www-igm.univ-mlv.fr/~dr/XPOSE2012/Integration%20Continue/concept.html
