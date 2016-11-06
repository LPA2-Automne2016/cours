# Les outils associés au CSS
## Les limitations du CSS

CSS n'est pas à proprement parler un langage de programmation.
Il s'agit simplement d'un ensemble d'instructions,
on ne peut pas faire de programmation avec CSS.

Les preprocesseurs CSS interviennent à ce niveau : Ils rendent possible
des habitudes de programmation et les transposent vers le CSS.

## Exemple d'utilisation:
Il est par exemple possible en SASS d'écrire :

> la classe .success hérite de la classe .message en ajoutant une couleur verte

```scss
.message {
  border: 1px solid #ccc;
  padding: 10px;
  color: #333;
}

.success {
  @extend .message;
  border-color: green;
}
```

Cela se traduit par le CSS suivant, après compilation :

```css
.message, .success {
  border: 1px solid #cccccc;
  padding: 10px;
  color: #333;
}

.success {
  border-color: green;
}

```

##  Les aides apportées par les preprocesseurs :

* Les Mixins vont permettre de rapporter un ensemble d'instructions à l'intérieur du bloc courant
* Héritage au sens développement objet.
* Utilisation de variables pour par exemple contenir les  couleurs
* Ecriture du CSS de façon hiérarchique.

## Les principaux prépreprocesseurs :
### SASS

http://sass-lang.com/

SASS est apparu en 2006, dans la lignée des avancées et de la ligne introduite par RAILS.
C'est le preprocesseur historique. Il est écrit en ruby et est intégré en standard dans RAILS.

### LESS

http://lesscss.org/

LESS est apparu en 2009 et était à l'origine écrit en ruby, mais a migré vers du JS.
Il est fortement influencé par SASS et en est très proche.
La différence notable est que vu qu'il est écrit en JS, il est possible de gérer la compilation en CSS directement dans le navigateur.
