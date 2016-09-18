# le modèle
<img src="http://www.montaignestyle.com/wp-content/uploads/2015/03/defile-elie-saab-printemps-ete-2015-paris-look-1_01.jpg" width="300">

**NON PAS DE RAPPORT**, d'aucun type d'ailleurs....

## La vraie utilité du modèle
Dans un MVC, le modèle est au coeur de la donnée et de leur manipulation. 
C'est ici qu'est concentrée toute l'intelligence de l'application. ( D'où d'ailleurs le fait qu'il n'y ait pas de rapport :-) )

Le modèle va être commun à toute l'application et sera partagé avec tous les controleurs. Une méthode en rapport avec une instance de la donnée ou bien une recherche potentiellement réutilisable sera inclue dans le modèle,  pour pouvoir s'en servir par ailleurs.

### Exemple 

Supposons qu'on travaille avec un modèle portant sur un utilisateur.
Le modèle contient :
* un nom
* un prénom 
* et une date de naissance
 
Si l'on demande une fonctionnalité qui n'est accessible que si l'utilsateur est majeur, on a deux options :

**Option 1** :imp: dans le controleur :
```ruby
def index()
    david = User.find_by(name: 'David')
    if david.birthday < Time.now - 18.years
        # code to display functionnality
    else
        # code to deny access
    end
end
```

**Option 2** :angel: dans le modele :
```ruby
class Student < ActiveRecord::Base
  def major?
    birthday < Time.now - 18.years
  end
end

# dans le controleur
def index()
    david = User.find_by(name: 'David')
    if david.major?
        # code to display functionnality
    else
        # code to deny access
    end
end
```

### Intérêt dans l'exemple
A priori, il s'agit d'une ligne de code assez innocente pour vérifier que l'utilisateur est majeur ou pas...
On pourrait donc sans trop d'impact la dupliquer dans les différents controleurs concernés par cette protection !

A priori, oui.... Sauf que... le client veut rendre l'application accessible aussi aux USA. Là-bas, l'âge légal est de 21 ans... Ceux qui ont eu le malheur de prendre l'option 1 doivent maintenant rouvrir tous leurs controleurs et tout revérifier. Ceux qui ont bien fait le travail n'ont qu'à modifier le modèle pour le prendre en compte !

références: http://guides.rubyonrails.org/active_record_basics.html

### Question BONUS 
Que manque-t-il dans l'exemple de code ci dessus ? (un indice: cela doit être un réflexe !)

Suite: [la vue](./03-la-vue.md)
