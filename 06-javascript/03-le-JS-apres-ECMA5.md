# Le JS apres ECMA 5

## Le contexte :
Les différents acteurs ont réussi à se mettre d'accord sur un standard pour Javascript. 
C'est la première fois dans l'histoire de ce langage !

L'écosystème devient mature, l'arrivée de Chrome sur le marché va bousculer encore plus les rapports de force : la V8 du moteur JS de chrome sur certaines applications va diviser par 8 les temps de réponse, forceant tout le monde à revoir sa copie pour rester dans la course ! 
La seconde guère mondiale du JS est lancée : après la première portant sur le Standard, **la deuxième porte sur la performance**. Elle est toujours en cours.

![chrome](https://www.google.com/googlebooks/chrome/images/small/1.jpg)

source: https://www.google.com/googlebooks/chrome/small_00.html

## Le résultat :
Les moteurs JS ont maintenant une richesse de sélecteurs, l'ajax se fait d'une façon unifiée. Les librairies comme JQuery ne sont plus strictement nécessaires ! Elles gardent certes une utilité, mais comparé à avant ECMA5, elle s'en trouve diminuée lorsque l'on n'a pas à supporter des navigateurs obsolètes.

Depuis 2012, on assiste à une nouvelle transformation :

```
Moteur JS plus rapide  + Javascript standardisé + API REST/webservice = Applications JS
```

L'avenir du développement web se porte maintenant vers des applications entièrement développée en JS et fonctionnant à l'intérieur du navigateur. Le principe est simple : le navigateur se charge de tout ce qui est lié à l'affichage (plus seulement du rendu des balises HTML, mais aussi de leur génération). Seule la  génération/le stockage des données est laissé à la charge du serveur.

Les fers-de-lance de cette vague :
* http://emberjs.com/
* https://angularjs.org/
* https://facebook.github.io/react/
* http://meteor.com

De plus, avec l'apparition de V8, le moteur JS de Chrome,  Ryan Dahl a eu l'idée de l'extraire pour en faire un serveur d'application. L'idée étant de permettre aux développeurs de développer leur applicaiton de A à Z en JS, que ce soit sur le serveur our le client !

# Le Javascript d'aujourd'hui

Le javascript d'aujourd'hui est maintenant piloté par les évolutions de l'ECMA, qui sont implémentées au fur et à mesure dans tous les navigateurs. Il a évolué pour ajouter la notion de classe, permettant ainsi aux développeurs Orienté Objet de se trouver en terrain famillier. Le langage est maintenant en train de rentrer dans une période de maturité.

# Le futur

le W3C vient d'annoncer le passage de WASM en tant que recommandation officielle, lui donnant du même titre le statut de "Standard de l'internet". Cela ouvre la porte à la compilation bas niveau ( pensez assembleur ), effaçant du même coup les barrières entre un client lourd et un navigateur, puisqu'avec WASM, les programmeurs ont maintenant accès à tout ce qu'il pouvaient faire en C dans un client lourd !


## Références :
* l'histoire du JS : https://resin.io/blog/happy-18th-birthday-javascript/
* https://learntocodetogether.com/javascript-es6-history/
* adoption de WASM par le W3C: https://www.w3.org/2019/12/pressrelease-wasm-rec.html.en
