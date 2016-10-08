# Le JS d'avant ECMASCript 5
## Contexte
Comme explicité avant, jusqu'en décembre 2009, javascript est au coeur de la mêlée générale, chaque éditeur ayant sa propre syntaxe et ou ses façons de faire, plus ou moins différentes selon les domaines. En décembre 2009, les différents protagonistes se mettent (enfin) d'accord. 
Cela donne naissance au standard ECMAScript 5 qui est le premier à être (dans l'ensemble) respecté.

De cette histoire vont naitre tout un écosystème de framework javascript dont la vocation principale est de protéger le développeur de toutes ces différences. Ces Framework vont de plus proposer des fonctions permettant de pallier aux insuffisances des navigateurs et du javascript.

## Quelques [librairies javascript][1] :
Par ordre chronologique d'apparition :
* [Jquery](https://jquery.com/) (2006)
* [MooTools](http://mootools.net/)(2007)

La librairie la plus répandue est de loin jquery, il est utilisé sur près de 65% des sites avec de gros traffics.

**NB: JQuery est une librairie js, il ne faut pas confondre avec le JS de base du navigateur**

Il arrive souvent de ne plus savoir faire la part des choses entre ce qui est du JS pur et ce qui provient de JQuery.

Exemple ```$('#myId')``` n'est valide que si JQuery est chargé ! 
Du fait des gains de temps que représente l'utilisation de JQuery par rapport à du JS natif, la très grande majorité des exemples donnés utilisera Jquery. **Gardez le bien à l'esprit ! Il s'agit d'exemples liés à une librairie, que vous n'aurez peut être pas dans la vraie vie !**