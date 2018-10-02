Variables
=========

Sython est un langage fortement type ainsi vous connaissez toujours le type de votre variable. De plus, les conversions ne sont pas implicite.

Déclaration
-----------

Actuellement, Sython comporte 3 types basiques différents :

- int, pour les entiers
- float, pour les nombres à virgules
- str, pour les chaines de caractères

Pour déclarer une variable, il faut suivre le paterne suivant : <type> <nom> = <valeur>

Exemple :

.. code-block:: python

    int entier = 1
    float flottant = 1.0
    str texte = "Bonjour"

.. note :: Comme vous avez pû l'apercevoir, les flottants n'utilise pas une virgule mais un point pour différencier la partie entière de la partie décimal

Affectation
-----------

Si vous voulez réaffecter une nouvelle valeur à votre variable, vous pouvez la redéclarer comme au-dessus mais il est plus économique d'utiliser le paterne suivant : <nom> = <valeur>

Exemple :

.. code-block:: python

    // Déclaration
    int entier = 1
    //Nouvelle affection
    entier = 2

.. note :: Ici, il y a aussi l'introduction des commentaires via le double symbole "//".
           
           Attention, les commentaires doivent être au début de la ligne et sans indentation.

Opérations
----------

Actuellement, Sython supporte 4 opérations :

- Addition : '+'
- Soustraction : '+'
- Multiplication : '*'
- Division : '/'

Ces opérations sont utilisables dans la déclaration et dans l'affection. Cependant, elles sont la cible de restriction :

- Il est impossible d'appliquer une opération sur deux valeurs de type différent (Pas de conversion implicite)
- Il est impossible de multiplier, diviser, soustraire deux chaines de caractères. Seul l'addition est possible avec ce type.
- Le resultat d'une division entre deux entiers n'est pas forcément un entier et peut entrainer une perte de données s'il est enregistré dans un entier

Exemple :

.. code-block:: python
  
    int entier1 = 2
    int entier2 = 3 + 4
    int entier3 = entier1 * entier2
    str phrase = "Bonjour "+"tout le monde"

Conversion
----------

Malgré le fait que les conversions ne peuvent être fait par Sython, vous pouvez les faire par vous même. La technique est tout simplement une déclaration avec le nouveau type.

Exemple :

.. code-block:: python
  
    str nombre = "1"
    // 'nombre' contient "1"
    int nombre = nombre
    // 'nombre' contient 1

.. note :: Attention, si la conversion n'est pas possible, vous aurez une erreur