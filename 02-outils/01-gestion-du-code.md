# La gestion du code: [le CVS](https://en.wikipedia.org/wiki/Version_control)
## L'enjeu :
Pour un développeur et plus généralement pour une entreprise réalisant des développements, le code et au travers lui les fonctionnalités qu'il permet sont sa richesse.
**Pour un développeur, la seule activité "rentable" est de produire du code.**

Les autres activités d'un développeur ne rapportent pas d'argent ! 
* générer des livrables
* installer des environnements
* débuguer 
* déployer des applications 
 
Ces activités sont certes obligatoires, mais aucun utilisateur ne va par exemple payer une fonctionnalité si l'application n'est pas déployée pour qu'il l'utilise. 
Par contre, l'utilisateur ne paye pas pour une installation, il paye une fonctionnalité.

La production du code et donc sa gestion sont donc le processus clef. Tout le reste est réduit au strict minimum, car non source de valeur ajoutée.

## Les outils d'hier et d'aujourd'hui:
Auparavant les gestionnaires de source permettaient une gestion "simple" du code source : exemple CVS, SVN.
Pas d'interaction particulière: on versionne et on sauvegarde du code en mode 'en ligne'.

Aujourd'hui les outils ont évolué vers du mode hors ligne avec la possibilité de versionner et de gérer du code même lorsque le PC n'est pas au réseau. 
Tous les gestionnaires de code proposent maintenant une très forte intégration avec les systèmes de gestions de bug, ainsi qu'une forte composante sociale. 
Le déploiement continu constitue maintenant la colonne vertébrale de ces systèmes.

### Quelques outils modernes pour la gestion du code :
* http://github.com
* https://bitbucket.org/
* https://about.gitlab.com/
 
[Le build et les dépendances](./02-le-build-les-dependances.md)