Permettra de rename de façon granulaire comme générale des chemins
<!-- TODO: Réecrire au propre cette doc pour correspondre à un man -->


Fonctionnalité
Etre en console
2 choix de fonctions : 
Le premier, rename un PATH absolu; Le deuxième, rename le contenu d'un dossier 

1 : rename un PATH absolu
Paramètre par défaut : 
-Suppression des espaces entre les mots + trim,
-Application du camelCase
Paramètre optionel : 
-Suppression des caractères spéciaux, pour remplacer par les caracs de la table ASCII

Avant le renommage afficher le résultat potentiel, proposer à l'user de valider le choix, ou d'annuler.


2 : rename le contenu d'un dossier
Paramètre par défaut : 
-Suppression des espaces entre les mots + trim,
-Application du camelCase
Paramètre optionel : 
-Suppression des caractères spéciaux, pour remplacer par les caracs de la table ASCII
-Récursivité, renomme tous les fichiers enfants du dossier courant. --depth, spécifie la profondeur à laquelle appliquer le renommage

Avant chaque renommage afficher le potentiel résultat, proposer à l'user de valider le choix, ou d'annuler.
Afficher chaque renommage sur une ligne numérotée 1, 2, ... n
Ainsi permettre à l'user d'annuler le renommage des numéros de ligne spécifiés

Choix 2: Possibilité d'ajouter la récursivité, c'est à dire que de base on rename juste le contenu direct du dossier, mais l'option récursivité on rename tout le contenu de chaque dossier.
Si récursivité prompt a chaque layer de dossier les protentiels résultats, et de proposer à l'user d'accepter ou de skip.
Si skip annuler les renames pour le contenu du dossier à depth=0, mais continuer de proposer pour les depth plus profondes.