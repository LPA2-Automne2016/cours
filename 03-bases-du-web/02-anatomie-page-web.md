# Anatomie d'une page web

## C'est quoi le HTML ?

Le HTML est le langage qui compose les pages web. L'abbréviation signifie **H**yper**T**ext**M**arkup**L**anguage. 
Un "markup language" est un language composé de balises ouvrantes et fermantes, comme par exemple ```<h1>ceci est un titre</h1>```
On retrouve le titre entouré de la balise ```<h1>``` et de sa balise fermante ```</h1>```

La liste des balises possible est définie par avance, ainsi que leur comportement. Vous trouverez [ici une liste (partielle) des balises de base](https://openclassrooms.com/courses/apprenez-a-creer-votre-site-web-avec-html5-et-css3/memento-des-balises-html), ainsi que leur utilité. 

Pour plus d'info, n'hésitez pas à suivre le tutorial : https://openclassrooms.com/courses/apprenez-a-creer-votre-site-web-avec-html5-et-css3

## Contenu d'une page :

Ceci est le strict minimun pour une page web valide :
```html
<!DOCTYPE html> <!-- indique au navigateur que la page est du HTML -->
<html> <!-- debut du document html--> 
    <head> <!-- début des entetes : les infos dans l'entete ne s'affichent pas, mais sont chargées en premier par le navigateur-->
        <!-- En-tête de la page -->
        <meta charset="utf-8" /> <!-- cette page est encodée en UTF8-->
        <title>Titre</title> <!-- le titre de la page, qui appparaitra dans l'onglet du navigateur-->
    </head>

    <body>
        <!-- Corps de la page -->
        <!-- ici va venir tout ce que vous voulez afficher-->
    </body>
</html>
```

**ATTENTION** Html est relativement contraignant : toute balise ouverte (ex: ```<h1>```) doit obligatoirement être fermée ensuite (```</h1>```).
Petite exception : une balise comme celle ci ```<meta charset="utf-8" />``` (notez le / à la fin de la balise) est à la fois ouvrante et fermante. 

les deux écritures sont donc équivalentes : ```<BR><BR/>``` est la meme chose que ```<BR/>```

## Le CSS dans tout ca ?

Avec l'arrivée du HTML 4, on a enfin eu accès au css. Avant HTML4, on mettait son texte dans la page web, et on mélangeait la présentation de ce texte avec. 

Exemple :

**ATTENTION CE QUI SUIT N EST PLUS VALIDE !!!! NE PAS FAIRE COMME CA !!!**

![catch](http://i.skyrock.net/0643/85670643/pics/3119899273_1_3_NVT9joQe.jpg)

```Avant, pour mettre un texte en gras, on faisait <b>comme ca</b on utilisait la balise <b> comme *BOLD* pour mettre en gras.```

**FIN DE CODE DANGEREUX A NE PAS UTILISER**

L'apparition du CSS a permis de séparer d'un coté le contenu de la page (le HTML) et de l'autre coté : la présentation qui est gérée par le CSS.
Pour se rendre compte de ce qu'on peut faire avec CSS : http://www.csszengarden.com/

Le HTML utilisé dans toutes ces pages est strictement le même ! Seul le CSS change.

# Le javascript cela sert à quoi ?

Le javascript apparait dans les premiers navigateurs, au début il était très limité. Maintenant il a énormément évolué, au point de pouvoir faire des serveurs web avec !
Il va servir à apporter des comportements dynamiques à l'intérieur de la page web.

Suite [les types de données](./03-les-types-de-donnees.md)
