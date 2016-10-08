# Un peu d'histoire
## Les navigateurs, le [javascript][1] :
![evolution js](https://www.visualnews.com/wp-content/uploads/2011/09/Interactive-Web-Browser-History-1.png)

http://evolutionofweb.appspot.com/

Le javascript apparait aux alentours de 1994, mais au début il n'est que très peu présent et très peu supporté.
Il a longtemps été la source d'un conflit entre les différents navigateurs, chaque éditeur ayant sa propre version de Javascript, avec ses propres instruction et ses avantages et faiblesses.
Il faut attendre la cinquième version du standard ECMA (es5) pour que les choses se stabilisent et convergent enfin !
Nous sommes alors aux alentours de 2011 :

![es5](./es5.PNG)

http://kangax.github.io/compat-table/es5/

## Le résultat :

![casse tete](http://static.canalblog.com/storagev1/littlesun.canalblog.com/images/marteau.gif)

Avant IE7 (pour rappel année 2006), pour un simple appel AJAX :
``` javascript
var xhttp;
if (window.XMLHttpRequest) {
    xhttp = new XMLHttpRequest();
    } else {
    // code for IE6, IE5
    xhttp = new ActiveXObject("Microsoft.XMLHTTP");
}
// 6 lignes, toujours pas de requête....
```
Il fallait créer un activeX pour pouvoir gérér cet appel. Comme les PC avec IE6 n'ont pas disparus instantanément à la sortie de IE7, cela signifie concrètement que pendant les années suivantes, il fallait encore gérer cette distinction !
Pour un développeur, supporter la panoplie des différents navigateurs en service relevait de la gageure !

Suite [le monde avant Chrome et ES5](./02-le-js-avant-chrome.md)

[1]:https://en.wikipedia.org/wiki/JavaScript