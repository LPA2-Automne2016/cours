# La base  du web : l'URL
<p align="center"> <img src="http://vignette1.wikia.nocookie.net/lotr/images/3/3f/One_Ring_To_Rule_Them_All.gif/revision/latest?cb=20131010232524"/><BR>
Three Rings for the Elven-kings under the sky,<BR/>
Seven for the Dwarf-lords in their halls of stone,<BR/>
Nine for Mortal Men doomed to die,<BR/>
One for the Dark Lord on his dark throne<BR/>
In the Land of Mordor where the Shadows lie.<BR/>
One Ring to rule them all, One Ring to find them,<BR/>
One Ring to bring them all and in the darkness bind them<BR/>
In the Land of Mordor where the Shadows lie.<BR/></p>

## Signification
URL signifie *"Uniform Resource Locator"*. Comme son nom l'indique l'URL sert de point d'entrée sur internet et sert à localiser des ressources (par ressource comprenez pages web dans notre cas).

**Attention**: les URLS ne se limitent pas à internet. 

Par exemple : *jdbc:postgresql://mydatabase.mydomain.com::5740/accounting* est une url valable. Elle ne représente pas une page web, mais une connexion à une base postgresql.

## Composition
Dans le cas du web, une URL s'ecrit de la façon suivante :  http://github.com:80/LPA2-Automne2016/cours/

Si on la décompose on retrouve :

| morceau                  | Signification                                      |
|--------------------------|----------------------------------------------------|
| http://                  | protocole http ou https si sécurisé                |
| github.com               | nom DNS du serveur                                 |
| :80                      | port du serveur, optionnel, si omis, alors 80      |
| /LPA2-Automne2016/cours/ | chemin à l'intérieur du serveur, defaut /          |

## Conseil 
**L'URL est ce qui est fait face à l'utilisateur** et ce qu'il doit taper dans le navigateur pour accéder à votre site web. 
Il est donc impératif d'y prendre garde et de **particulièrement soigner sa présentation**.

Personne ne voudrait avoir à taper une URL du genre

http://github-example-4269.herokuapp.com/projects/1237576/file/1684721 

pour en réalité accéder au fichier 

http://github.com/LPA2-Automne2016/cours/00-la-base-du-web-URL.md

La deuxième variante est beaucoup plus pratique, même si en pratique, dans la représentation physique du site web de github, elle doit plus se rapprocher de la première variante.

**Moralité**: pour satisfaire les besoins de l'utilisateur, soignez vos URLs !

Suite: [Comment fonctionne le navigateur](01-comment-fonctionne-le-navigateur.md)