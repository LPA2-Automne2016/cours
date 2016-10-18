# Le JS d'avant ECMASCript 5
## Contexte
Comme explicité avant, jusqu'en décembre 2009, javascript est au coeur de la mêlée générale, chaque éditeur ayant sa propre syntaxe et ou ses façons de faire, plus ou moins différentes selon les domaines. En décembre 2009, les différents protagonistes se mettent (enfin) d'accord. 
Cela donne naissance au standard ECMAScript 5 qui est le premier à être (dans l'ensemble) respecté.

De cette histoire vont naitre tout un écosystème de framework javascript dont la vocation principale est de protéger le développeur de toutes ces différences. Ces Framework vont de plus proposer des fonctions permettant de pallier aux insuffisances des navigateurs et du javascript.

## Quelques [librairies javascript][1] :
Par ordre chronologique d'apparition :
* [JQuery](https://jquery.com/) (2006)
* [MooTools](http://mootools.net/)(2007)

La librairie la plus répandue est de loin JQuery, elle est utilisée sur près de 65% des sites avec de gros traffics.

**NB: JQuery est une librairie js, il ne faut pas confondre avec le JS de base du navigateur**

Il arrive souvent de ne plus savoir faire la part des choses entre ce qui est du JS pur et ce qui provient de JQuery.

Exemple ```$('#myId')``` n'est valide que si JQuery est chargé ! 
Du fait des gains de temps que représente l'utilisation de JQuery par rapport à du JS natif, la très grande majorité des exemples donnés utilisera Jquery. **Gardez le bien à l'esprit ! Il s'agit d'exemples liés à une librairie, que vous n'aurez peut être pas dans la vraie vie !**

# Introduction à JQuery
JQuery a commencé à ses débuts avec une promesse majeure : permettre au développeur de ne pas se préoccupper de savoir sur quel navigateur son code sera exécuté.

## Ses forces:  
* Une gestion de l'ajax indépendante du navigateur
* Des sélecteurs très perfectionnés

## Exemple 
https://jsfiddle.net/ts79gb0q/

```html
<input id="myInput">
<button>click me !</button>
<div id='result'>
</div>
```

```javascript
$("button").click(function() {
  var txt = $("#myInput").val();
  alert(txt);
 	$.ajax({  url: "/echo/json/",
            type: "POST",
            contentType: "application/json", // send as JSON
            data: {json: JSON.stringify({ value: txt})},
            success: function(data) {
               console.log(data);
               $('#result').html(data.value);
            }
         });
});
```

Tout cela a changé avec l'arrivée de l'ECMASCRIPT5, [Suite...](./03-le-JS-apres-ECMA5.md)

[1]:https://en.wikipedia.org/wiki/List_of_JavaScript_libraries
