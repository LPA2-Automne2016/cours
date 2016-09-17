# Le controleur
![le controleur](
http://www.defense.gouv.fr/var/dicod/storage/images/base-de-medias/images/air/actualites/images-2012/images-janvier-20122/controleurs-aeriens-de-l-armee-de-l-air/1538332-1-fre-FR/controleurs-aeriens-de-l-armee-de-l-air.jpg)
**CA par contre, ca a un rapport  !**

## Utilité du controleur:
Le controleur est chargé d'accepter les requêtes qui arrivent au serveur d'application. Lorsqu'une requête arrive, elle va invoquer la méthode correspondante sur le controleur. Le travail du controleur va alors consister à :
* interroger le modèle de données pour récupérer les données nécessaires à la vue.
* Choisir le type de vue nécessaire à l'appelant (JSON/XML/HTML/autre)
* Fournir les données à la vue et déclencher le rendu

## Précautions à prendre

Les controleurs doivent être les plus "fins" possible (règle du pouce). La raison est la suivante : on l'a vu dans leur définition de base, les controleurs sont liés à une seule page. Toute intelligence qu'on y mettrait serait alors perdue pour les autres pages et devrait donc être réécrite. 

D'une façon générale, l'ensemble du développement de l'application s'efforce de suivre le principe **DRY** *Don't Repeat Yourself*.

C'est un principe de base dans le développement qui dit que si vous devez répéter du code, c'est qu'il y a une erreur de conception quelque part. **Copier/Coller est l'ennemi du développeur !**

Référence : http://guides.rubyonrails.org/action_controller_overview.html