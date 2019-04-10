
# Corewar Electronique - Cahier des charges
___

## Contexte

Le Corewar est un jeu dans lequel les joueurs font combattre des programes appeles *Champions*.
La conception de la machine virtuelle servant d'arrene de combat pour ces champions est aussi un [project de 42](https://projects.intra.42.fr/projects/corewar).  
Le championchip du Corewar le rend aussi tres populaire chez les étudiants de 42. Pour répondre a l'amour des étudiants pour ce jeu, nous proposons de realiser une version physique de l'arrene de combat. Celle-ce permetteras ainsi l'affrontement de champions, celon les regles du Corewar de 42, sur un support original.  

## Contraintes

### Chargement des champions
Un tel Corewar doit proposer un systeme simple, pratique et rapide pour charger les champions destines a s affronter.  
Pour cela, nous pensons utiliser un systeme de lecture de cartes, par exemple RFID.
Les champions devront etre prealablement compiles, puis ecrit sur les cartes, avant de pouvoir etre passe devant un dispositif de lecture, si possible, sans contact.  
Il devras etre possible de charger au moins 2 champions.  

### Les Regles des combat
L'arrene serras implementee de facon a pouvoir etre reprogramable en cas de changement mineur des regles du corewar, sans modifications physique.  
Dans le cas de changements importants des regles pendant la conception du Corewar Electronique, il est possible que nous utilisions les regles effectives en 2018.  

### Affichage
Le Corewar Electronique devras proposer une visualisation des combats en cours.  
Pour des raisons de visibilite, un affichage avec une resolution minimum de 32x32 serras necessaire (neamoins un affichage en 64x64 permetterrais d'afficher l'integralitee de la memoire). Le taux de rafraichissement devras etre raisonable.  
Visuel en 32x32 led rgb minimum, avec écran d'information affichant les noms, aff et jours de règne du grand champion actuel de l'arène (hors combat).  
Un affichage de type textuel permettrais d'afficher des details de maniere lisible, tel que le nom des champions.  

## Fonctionnalitees secondaires
Celles-ci serront implementees des que possible mais ne constituent pas l'objectif principal du projet.

### Le grand champion de l'arrene
Ceci est un mode de jeu ajouttant de l'interet a une arrene de Corewar physique.  
Bien qu'il pourrait etre possible de charger plusieurs champions pour les faire se combattre, il serra egalement possible de n'en charger qu'un, qui affronterra alors le dernier gagnant du mode "Grand champion de l'arrene". Celui-ci pourras alors accumuler des statistiques tels que le nombre d'adversaires vaincus, et etre affiche dans l'arrene.  
Bien entendu, les gagnants du mode "Simple Combat" ne serront pas enregistres dans l'arrene.  

### Controls avances
Des controls additionels permetterraient de simplifier certaines utilisations:
- Un bouton pour changer de mode.
- Une procedure pour reinitialiser l'arrene (probablement pas un bouton, car cela permetterrais de tricher... peutetre utiliser un code special a la place, implemente dans le code de l'arrene ?).
- Un bouton pour mettre en pause, ou executer au ralentis.
