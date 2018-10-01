Entrée - Sortie
===============

C'est bien de créer des variables mais il est mieux d'afficher quelque chose nan ?

Affichage
---------

L'affichage est très simple : il utilise la fonction 'show()' qui prend un seul paramètre.

Exemples :

.. code-block :: python
    
    //Le bon vieux 'Hello World'
    show("Hello World")

.. code-block :: python

    //Ce code va calculer le resultat de 2 + 2 puis l'afficher
    int result = 2 + 2
    //Ici la conversion est nécessaire pour additionner deux str entre eux
    str result = result
    show("Le résultat de 2 + 2 est "+result)

.. note :: Comme vous avez pû le voir, les additions (et autres opérations) sont possibles dans la fonction 'show()'

Interaction
-----------

Afficher des trucs est sympa mais si nous voulons récupérer des informations écrites par l'utilisateur ?

C'est simple, la fonction 'enter()' est faite pour vous ! Celle ci prend un seul paramètre.

Exemples :

.. code-block :: python

    str name = enter("Entrez votre nom : ")
    show("Votre nom est "+name)

.. code-block :: python

    int age = enter("Entrez votre age : ")
    str age = age
    show("Vous avez "+age+" ans")

.. note :: Dans notre deuxième code, la variable 'age' est d'abord un int. Ceci permet que l'utilisateur ne rendre que des entiers, s'il ne le fait pas, le programmation crashera.

           Il est prévu de rajouter des fonctions pour vérifier si un str peut être convertit en entier / flottant.
