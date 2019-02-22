# Le JS apres ECMA 5

## Le contexte :
Les différents acteurs ont réussi à se mettre d'accord sur un standard pour Javascript. 
C'est la première fois dans l'histoire de ce langage !

L'écosystème devient mature, l'arrivée de Chrome sur le marché va bousculer encore plus les rapports de force : la V8 du moteur JS de chrome sur certaines applications va diviser par 8 les temps de réponse, forçant tout le monde à revoir sa copie pour rester dans la course ! 
La seconde guère mondiale du JS est lancée : après la première portant sur le Standard, **la deuxième porte sur la performance**. Elle est toujours en cours.

![chrome](https://www.google.com/googlebooks/chrome/images/small/1.jpg)

source: https://www.google.com/googlebooks/chrome/small_00.html

## Le résultat :
Les moteurs JS ont maintenant une richesse de sélecteurs, l'AJAX se fait d'une façon unifiée. Les librairies comme JQuery ne sont plus strictement nécessaires ! Elles gardent certes une utilité, mais comparé à avant ECMA5, elle s'en trouve diminuée lorsque l'on n'a pas à supporter des navigateurs obsolètes.

Depuis 2012, on assiste à une nouvelle transformation :

```
Moteur JS plus rapide  + Javascript standardisé + API REST/webservice = Applications JS
```

L'avenir du développement web se porte maintenant vers des applications entièrement développées en JS et fonctionnant à l'intérieur du navigateur. Le principe est simple : le navigateur se charge de tout ce qui est lié à l'affichage (plus seulement du rendu des balises HTML, mais aussi de leur génération). Seule la  génération/le stockage des données est laissé à la charge du serveur.

Les fers-de-lance de cette vague :
* http://emberjs.com/
* https://angularjs.org/
* https://facebook.github.io/react/
* http://meteor.com

De plus, avec l'apparition de V8, le moteur JS de Chrome,  Ryan Dahl a eu l'idée de l'extraire pour en faire un serveur d'application. L'idée étant de permettre aux développeurs de développer leur applicaiton de A à Z en JS, que ce soit sur le serveur ou le client !

# Le futur : ECMA6
![peinture fraiche](http://www.pro-signalisation.fr/21225-product_prosignalisation/chevalet-caution-peinture-fraiche.jpg?frz-v10)

Le nouveau standard ECMA6 a été validé en 2015, il est en cours d'implémentation dans les navigateurs, et va apporter beaucoup de nouveautés pour faciliter encore le développement JS.

Liste des évolutions: http://es6-features.org/


## Références :
* l'histoire du JS : https://resin.io/blog/happy-18th-birthday-javascript/
