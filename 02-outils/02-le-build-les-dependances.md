# Le build et la gestion des dépendances
## Contenu et utilité

Le build couvre les différentes étapes suivantes:
* la mise à jour et le téléchargement des dépendances
* la constitution des binaires utiles pour le déploiement
* le lancement des différentes suites de test : ( unitaire, intégration, acceptation)
 
Il peut par ailleurs dans certains cas inclure des tâches de déploiement du code et/ou des utilitaires utilisés pour des actions répétitives dans les travaux de développement. 
Comme évoqué précédement, l'objectif est d'automatiser ce qui peut l'être pour que le temps soit le plus possible passé sur les activités génératrices de valeur : le développement proprement dit.

## Choix du système de build

Le choix du système de build est très fortement influencé par le choix du framework et de la technologie de développement.
En effet chaque langage/framework est livré avec son build, le choix est donc assez restreint.

## Quelques logiciels de build/gestion de dépendance

Selon le langage et le framework, parfois la gestion des dépendances est externalisée par rapport au build proprement dit.
Selon les cas, il peut arriver que le même fichier/logiciel de build remplisse les deux fonctions

| langage                 | Build                                                    |
|-------------------------|----------------------------------------------------------|
| [ruby][0] / [rails][1]  | [rake][2], [bundler][3], [gem][4]                        |
| java / [spring][5]      | [maven][6], [gradle][7] , ant , ivy (sous projet de ant) |
| nodejs                  | npm, gruntjs, bower                                         |
| groovy / [grails][8]    | [gradle][7]                                              |
| scala / [play][9]       | sbt                                                      |
 
En dehors des logiciels cités ci-dessous, il existe également Xooctory, créé en mars 2007 avec la collaboration de l'Université Bordeaux I. Xooctory permet, en plus de la gestion des dépendances: 
* un reporting instantané
* une gestion avancée des droits 



Sources: http://dept-info.labri.u-bordeaux.fr/~baudon/Master/TLA/Hanin.pdf
         http://blog.soat.fr/2014/08/bower-un-gestionnaire-de-dependances-pour-le-web/ (plus de détails sur bower)
 
## La morale de l'affaire:

![pourquoi faire simple quand c'est si simple de faire compliqué](http://img3.bibamagazine.fr/var/bibamagazine/storage/images/media/images/culture/20150505-10-citations/les-shadoks-8/292381-1-fre-FR/Les-Shadoks-8_max1024x768.jpg)


Utiliser un système de build lié à son écosystème de développement **peut au premier abord paraître inutile** : en effet on pourrait très bien tout faire à la main ?? 

**FAUX : il y a une vie après l'UV de LPA2 !!! si vous devez reprendre le code 6 mois plus tard, vous ne vous rappelerez plus de comment tout installer.** Mieux vaut passer quelques heures de plus sur le sujet aujourd'hui et s'épargner des jours plus tard.

Suite [L'intégration continue](03-integration-continue.md)

[0]:https://www.ruby-lang.org/fr/
[1]:http://rubyonrails.org/
[2]:http://rake.rubyforge.org/files/doc/rational_rdoc.html
[3]:http://bundler.io/
[4]:https://rubygems.org/
[5]:https://spring.io/
[6]:https://maven.apache.org/
[7]:https://gradle.org/
[8]:https://grails.org/
[9]:https://www.playframework.com/
