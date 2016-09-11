# Le [déploiement continu][CD]

Le déploiement continu se situe dans la prolongation de l'intégration continue.
Il s'agit de déployer automatiquement le code si les différents tests passent.

Encore une fois, l'accent est mis sur les tests. Il est même parfois possible lorsque la pratique est poussée à l'extrême d'aller jusqu'à des déploiements automatisés sans validation humaine.

![continuous Delivery Pipeline](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Continuous_Delivery_process_diagram.svg/731px-Continuous_Delivery_process_diagram.svg.png)

Source : https://en.wikipedia.org/wiki/Continuous_delivery

## Les différentes variantes

Le coeur de la pratique consiste toujours à livrer soit depuis le CVS directement, soit en passant par l'IC.
Les différentes parties de l'application sont générées et déployées sur les serveurs servant soit de qualification, soit directement de production. On retrouve des variantes dans le degré d'automatisme des processus: avec ou sans validation humaine.

## Techniques connexes

L'automatisation promue par ce processus impose un certain nombre de contraintes sur l'architecture serveur. L'objectif étant de tout déployer en un clic, il n'est pas envisageable d'installer des serveurs à la main. 
Ceci est rendu possible par un certain nombre de technologies qu'il est fortement conseillé de connaître pour un développeur.
Ces technologies ne font pas partie du périmètre du cours, mais sont néanmoins essentielles :

* Docker: https://www.docker.com/
* Chef : https://www.chef.io/chef/
* Ansible : https://www.ansible.com/
* vagrant : https://www.vagrantup.com/
 
Suite : [le choix du framework](./05-le-framework.md)

[CD]:https://en.wikipedia.org/wiki/Continuous_delivery
