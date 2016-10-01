# Les webservices

## L'origine
![genèse](http://www.lemondedesreligions.fr/images/2011/05/19/1516_bible_440x260.jpg)

**Au commencement, Microsoft et UserLand Software créèrent [XML-RPC][1]**

Aux alentours des années 1998, internet est en plein essor, la volonté de pouvoir interagir entre système est déja présente, 
mais jusque là limitée à des échanges au sein d'un même langage ou plateforme exemple [RMI][2] pour java, [COM][3] pour windows.
Microsoft et UserLand Software se rapprochent alors pour mettre au point un protocole circulant sur HTTP, et sérialisé en XML.
L'avantage est énorme : tous les langages savent "parler" HTTP, ils savent tous désérialiser du XML. 

Résultat **XML-RPC est né, il est utilisable par tout le monde, quelque soit le langage de programmation et ou son OS**

XML-RPC a ensuite évolué SOAP

![XML-RPC](https://img.pokemondb.net/artwork/tentacool.jpg) ![->](https://cdn4.iconfinder.com/data/icons/ionicons/512/icon-arrow-right-b-128.png) ![SOAP](https://img.pokemondb.net/artwork/tentacruel.jpg)


## La situation aujourd'hui

Comme évoqué avant : SOAP est à la base du XML au travers de HTTP. 
Au dessus de tout cela, il y a une couche permettant de décrire les méthodes qui peuvent être appelées, leurs entrées/sorties.
Il s'agit du WSDL qui un fichier XML décrivant les méthodes, leurs paramètres, etc.

En résumé : **SOAP est relativement lourd à mettre en place**, il est néanmoins encore utilisé, car il est rigoureux.

## L'alternative : REST

Face à cette relative complexité de SOAP s'est développée une alternative plus simple : [REST](../03-bases-du-web/04-les-verbes-http.md). 
*rappelez vous, nous en avons parlé à la dernière séance*

Le principe et simple : 
* on utilise l'URI
* un verbe HTTP pour signifier l'intention 
* on sérialise tout en JSON pour économiser la bande passante.

Pas de descriptif de méthode comme dans SOAP

Aujourd'hui, quasi tous les webservices sont disponibles en REST

Suite : [quelques exemples](./02-exemples.md)


[1]:https://en.wikipedia.org/wiki/XML-RPC
[2]:https://en.wikipedia.org/wiki/Java_remote_method_invocation
[3]:https://en.wikipedia.org/wiki/Component_Object_Model
