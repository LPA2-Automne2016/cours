# C'est quoi un navigateur ?

## [Le fonctionnement de base du navigateur:](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/HTTP_Basics.html)

Le navigateur ne fait pas de magie : tout se passe sur le réseau.  le navigateur interroge le serveur distant sur une socket, récupère la réponse, l'interprète, et l'affiche.

![http browser](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP_Steps.png)

source : https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP_Steps.png

## Exemple de requête web:

![requete http](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP_RequestMessageExample.png)

La requête contient, par ordre d'apparition :
* **un Verbe (GET)**, **un chemin (/doc/test.html)**, un protocole (HTTP/1.1)
* l'hôte auquel s'adresse la requete (www.test101.com)
* les headers
* une ligne vide pour marquer la fin de la requête
* un corps de message qui suit (optionnel)

Plus de détails : https://tools.ietf.org/html/rfc2616

## Exemple de réponse:

![reponse](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP_ResponseMessageExample.png)

On retrouve dans la réponse :
* le protocole (HTTP/1.1), **le statut** (200 OK)
* des headers 
* une ligne blanche
* le contenu de la page (optionnel, mais très fréquemment rempli)
 
plus de détails : https://tools.ietf.org/html/rfc7231

Dans l'exemple ci dessus, la partie qui nous intéresse et qui fera l'objet du travail est 

```<h1> My Home page</h1>```

suite : [anatomie d'une page web](./02-anatomie-page-web.md)
