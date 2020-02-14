# Encore un peu d'histoire
## Apparition du CSS
![evolution js](https://c7.uihere.com/files/630/729/169/web-browser-web-application-internet-evolution-timeline.jpg)

http://evolutionofweb.appspot.com/

Le CSS apparait en 1996 sur IE, mais n'est que très partiellement implémenté.
Il faut attendre les environs de l'année 2000 pour qu'il soit vraiment implémenté
et commence à être utilisé par les développeurs.

## Principe de base du CSS:

Le CSS répond au principe de  base suivant : **Séparer le fond de la forme**.

Il s'agit de pouvoir mettre d'un coté les code qui compose le contenu de la page web.
Et d'isoler dans un autre contexte/emplacement les détails liés à la présentation de ce contenu.

## Historique du CSS

Pour exactement les mêmes raison et de la même façon que pour le JS,
le CSS a été victime de son histoire avec des comportements, des syntaxes variant d'un navigateur à l'autre !

Exemple un arrondit de coin sur une div :

```css
.box {
  -khtml-border-radius: 10px; /* Konkeror unix */
  -webkit-border-radius: 10px; /* Apple Safari*/
  -moz-border-radius: 10px; /* Firefox */
  -ms-border-radius: 10px; /* IE avant < 9*/
  border-radius: 10px;
}
```

Ceci est un VRAI exemple... **5 syntaxes différentes** pour un coin arrondi sur une div...

Avis à ceux qui veulent réinventer la roue !

![i m watching you](http://1.bp.blogspot.com/-eZbb42e4T-U/U5f5Fey3akI/AAAAAAAAItc/XtVplSNFbwQ/s1600/watching-you.png)


Suite [les enjeux](02-les-enjeux-du-CSS.md)
