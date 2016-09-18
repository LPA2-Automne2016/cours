# La vue
## Utilité
Dans un MVC, la vue est chargée de l'affichage des données à destination de l'utilisateur. Il n'y a aucune intelligence dans une vue.
Le principe d'une vue est qu'elle va recevoir de la part du controleur la liste des données à afficher et elle les mettra en forme.

## Exemple d'utilisation:
C'est là qu'on retrouve le fameux HTML. Ni le controleur ni le modèle ne s'occuppent de la façon dont doit être affichée la donnée, il s'agit du travail de la vue. 

Par exemple, une vue pourra à partir d'une liste d'étudiant :
* afficher un tableau avec leurs différentes caractéristiques
* en faire une liste à puce
* utiliser cette liste pour remplir une liste déroulante dans un formulaire
* extraire cette liste au format JSON
* extraire cette liste au format XML

## Quelques types de vue
La vue prépondérante est celle qui produit du HTML, mais ce n'est pas tout.
Les vues peuvent aussi produire (liste non exhaustive)
* du JSON
* du XML
* des fichiers : PDF, EXCEL, CSV, WORD...
 
Références : http://guides.rubyonrails.org/layouts_and_rendering.html

Suite : [le controleur](./04-le-controller.md)
