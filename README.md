La gestion d'un formulaire par le code repose sur quatre classes principales :

    AbstractControl, c'est la classe-mère de tous les contrôles. C'est elle qui apporte toutes les propriétés permettant d'accéder à l'état, aux erreurs, aux valeurs des différents types de contrôle.

    FormControl est un objet amené à gérer l'un des éléments du formulaire (input ou select), à traquer ses changements de valeur, son état, la validation des données qui y sont associées, etc.

    FormGroup regroupe un ensemble d'objets de type AbstractControl sous forme d'objet. Il peut contenir contenir 1 à n AbstractControl. Un FormGroup peut être imbriqué dans un autre FormGroup afin de mutualiser les règles ou valider, selon les valeurs de plusieurs contrôles.

    FormArray regroupe un ensemble d'objets de type AbstractControl sous forme de tableau. Chaque contrôle est identifié par un index.

    ValidatorFn est une fonction qui représente une règle de validation

_Remarque : les classes FormControl, FormGroup, FormArray héritent toutes de la classe _AbstractControl
