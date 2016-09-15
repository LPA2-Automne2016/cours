# Les différents types de données

## Le pourquoi

Dans le chapitre précédent, nous avons évoqué :
| Type de donnée | Utilité                     |
|----------------|-----------------------------|
| HTML           | Structure de la page web    |
| CSS            | Présentation de la page     |
| Javascript     | Comportement dynamique      |

Ces 3 composants s'additionnent pour former la page web telle qu'on la connait. Cependant, dans le cadre de certaines fonctionnalités d'une page web il est souvent nécessaire de faire appel à de la donnée qui ne fait pas partie de la page web en tant que telle, mais doit être chargée depuis l'extérieur.

On fait alors transiter de la donnée "pure" sur le réseau. L'objectif de ce transfert est de faire circuler uniquement la donnée et non pas l'intégralité de la page web, ceci afin de gagner en temps de transfert et/ou en fluidité.

**Exemple d'utilisation :**

Lorsque l'on tape le début d'une phrase dans la boite de recherche google, on vous propose le reste de la phrase. La page n'est pas rechargée et elle ne contient pas toutes les possibilités (elle mettrait 2 jours à charger :-) ). Cette technologie s'appelle l'[AJAX](http://www.w3schools.com/ajax/) et permet de charger des données en arrière plan.

## Le comment 

Les données sont transmises dans un format appelé JSON, qui combine une très grande simplicité avec un faible encombrement sur le réseau.

* Une Map sera représentée ainsi : ```{clef:'valeur', autreClef: 3}```
* Une liste sera représentée ainsi ```[1, 2, "une chaine de charactères"]```

Ceci permet très simplement de représenter des objects complexes: 
*(indenté ici pour être plus lisible, en réalité tout sur une même ligne dans la pratique)*

```json
{  
    uv: { 
        nom: 'LPA2', 
        enseignant: 'Sebastien Gadot', 
        modalites: {
            frequence: "tous les mardis",
            typesDeCours: [ "cours", "TD", "TP" ]
        }
    }
}
```

Nous verrons plus tard la façon dont on utilise cette donnée et comment la récupérer/interroger le serveur via Javascript.

Suite : [les verbes HTTP]:(./04-les-verbes-http.md)