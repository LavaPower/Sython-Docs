Conditions
==========

Tests
-----

Avant de créer des conditions avec des 'if'... Il faut d'abord créer des tests.

Les tests sont des objets dont on veut savoir s'il est vrai ou pas.

En Sython, ces tests peuvent être :

- Une simple valeur / variable -> Il suffit de mettre la valeur ou le nom de la variable
- Une égalité entre deux valeurs -> If suffit de suivre ce paterne : '<valeur/variable> == <valeur/variable>'
- Une inégalité entre valeurs -> Il suffit d'utiliser des signes '<=' '>=' '<' '>' dans le parterne du haut à la place de '=='

If
---

Commençons par la condition la plus simple : 'si <...> alors <...>'. En Sython, la synthaxe se démarque de Python avec l'utilisation d'accolade :

.. code-block :: python

    if <test> {
        <code>
    }

.. note :: Le placement des accolades est à respecter, de plus, l'indentation ne peut se faire que via des espaces pour l'instant.

Exemple :

.. code-block :: python

    int a = 1
    if a == 1 {
        show("a = 1")
    }

.. note :: Ce code affichera 'a = 1'

Elif
----

En complémentarité du 'if', ce trouve 'elif'. Celui-ci correspond en français à 'sinon si <...> alors <...>' et s'utilise comme le if.

.. code-block :: python

    if <test> {
        <code>
    }
    elif <test> {
        <code>
    }

Exemple :

.. code-block :: python

    int age = enter("Entrez votre age : ")
    if age > 18 {
        show("Vous êtes majeur depuis au moins un an !")
    }
    elif age == 18 {
        show("Vous êtes majeur depuis moins d'une année ! Bravo à vous !")
    }

.. note :: Attention : Dans ce code, si l'utilisateur entre un nombre inférieur à 18, rien ne s'affichera mais nous allons y remédier.

Else
----

Le dernier du trio gagnant est le 'else'. Il correspond à 'sinon' et lui n'a pas de test, il sera vrai si les tests du haut sont faux.

.. code-block :: python

    if <test> {
        <code>
    }
    elif <test> {
        <code>
    }
    else {
        <code>
    }

Exemple :

.. code-block :: python

    int age = enter("Entrez votre age : ")
    if age > 18 {
        show("Vous êtes majeur depuis au moins un an !")
    }
    elif age == 18 {
        show("Vous êtes majeur depuis moins d'une année ! Bravo à vous !")
    }
    else {
        show("Vous êtes mineur, profitez !")
    }