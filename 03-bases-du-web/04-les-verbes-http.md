# Les verbes HTTP et leur importance
## Petit rappel 

![http browser](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP_Steps.png)

Le verbe HTTP est le premier mot de la trame échangée entre le navigateur et le servuer (ici étape 2)

## Les verbes HTTP
[La norme HTTP](https://tools.ietf.org/html/rfc7231) crée les 8 verbes HTTP suivants, complété [par la suite](https://tools.ietf.org/html/rfc5789) par un 9eme .

* **GET** Action par défaut du navigateur
* HEAD
* **POST**  Création d'un nouvel élément
* **PUT** Modification d'un élément (remplacé par PATCH)
* **DELETE** Suppression d'un élément
* CONNECT
* OPTIONS
* TRACE
* **PATCH** Modification d'un élément
 
Les verbes en gras sont les plus utilisés et les plus importants, car ils ont une signification particulière dans le cadre des développements.

## Le concept REST : *REpresentational State Transfer*
![REST](http://headstartsport.co.za/wp-content/uploads/2013/12/High-performance-rest.jpg)

*The term representational state transfer was introduced and defined in 2000 by Roy Fielding in his doctoral dissertation at UC Irvine. REST has been applied to describe desired web architecture, to identify existing problems, to compare alternative solutions and to ensure that protocol extensions would not violate the core constraints that make the web successful. Fielding used REST to design HTTP 1.1 and Uniform Resource Identifiers (URI).*

*The name "representational state transfer" is intended to evoke an image of how a well-designed Web application behaves: a network of web pages (a virtual state-machine), where the user progresses through the application by selecting links (state transitions), resulting in the next page (representing the next state of the application) being transferred to the user and rendered for their use.*

*To the extent that systems conform to the constraints of REST they can be called RESTful. **RESTful systems typically, but not always, communicate over Hypertext Transfer Protocol (HTTP) with the same HTTP verbs (GET, POST, PUT, DELETE, etc.) that web browsers use to retrieve web pages and to send data to remote servers**. REST systems interface with external systems as web resources identified by Uniform Resource Identifiers (URIs), for example /people/tom, which can be operated upon using standard verbs such as GET /people/tom.*

source : https://en.wikipedia.org/wiki/Representational_state_transfer

## La façon de s'en servir au sein de RAILS

![routing](https://camo.githubusercontent.com/f4c1e24418a2ff3d1e2cda182a4d0a4a541134c5/687474703a2f2f692e696d6775722e636f6d2f3067365a534d522e706e67)

Source: http://guides.rubyonrails.org/routing.html

Suite: [les headers](./05-les-headers.md)