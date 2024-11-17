Tutorial
--------

### Types de données

Le C++ propose une liste riche de types pré-définis, ainsi que des types définis par l'utilisateur. La liste suivante montre les sept types de données de bases en C++:

#### Pré-défini
* Booléen - `boolean` - soit `true` (vrai) ou `false` (faux)
* Caractères - les alphabets et tous les symboles. Défini via `char`.
* Entiers - nombres entiers qui peuvent soient être positifs ou négatifs. Défini via `int` (4 octets) ou `short int` (2 octets) ou `long int` (8 octets) en fonction de la taille des nombres utilisés.
* Nombres à point flottant - Nombres réels (nombres à fractions). Défini avec `float` et `double`.
* Sans valeur avec le mot-clé `void`
* Caractères longs avec le mot-clé `wchar_t`


#### Type Modifiers

Les types ci-dessus peuvent être modifiés avec les modificateurs de type suivants :
* `signed` et `unsigned`
* `short` et `long`

#### Définis par l'utilisateur
* Structures - `struct` sera expliqué plus tard, dans la section Structures.
* Classes - `class` sera expliqué plus tard, dans la section Classes.

C++ permet à une liste de caractères de définir du texte. Il procure aussi une grande librairie `string` pour manipuler du texte et sera expliqué dans la section Strings.

#### Définitions de type
Les Typedef (définition de type) permettent de créer de nouveaux noms (pensez-y comme des alias) pour des types existants. Ci-dessous est un exemple pour définir un nouveau type avec typedef:

    typedef int counter;
    counter tick_c = 100;  // tick_c est une variable entière valide

#### Types énumérés

Pour créer une énumération requiert le mot-clé `enum`. La forme générale d'un type énuméré est:

    enum nom_enum { liste de noms } var_list;
Ci-dessus, `nom_enum` est le nom de la variable à type énuméré. La liste de noms est séparé par des virgules.

Par exemple, le code suivant défini une énumération de couleurs appelée couleurs et la variable `une_couleur` de type couleur. Enfin, `une_couleur` est assignée la valeur "vert".

    enum couleur {rouge, vert, bleu} une_couleur, une_autre_couleur;
    une_couleur = green;  // une_couleur sera assignée la valeur de '1'

### Définir des variables

Pour les nombres, nous verrons principalement le type `int`, qui est un entier d'une taille d'un "word" la taille de nombre par défaut de la machine sur laquelle votre programme est compilé. Sur la plupart des ordinateurs aujourd'hui, c'est un nombre à 32 bits, ce qui signifie que les nombres peuvent avoir une valeur entre -2,147,483,648 et 2,147,483,647 (même chose pour `long`).

Pour définir les variables `foo` et `bar`, on utilise la syntaxe suivante:

    int foo;
    int bar = 1;

La variable `foo` peut être utilisée, mais parce-que nous ne l'avons pas initialisé, nous ne savons pas ce qu'il y a dedans. La variable `bar` contient le nombre 1.

Maintenant, on peut faire des maths. En supposant que `a`, `b`, `c`, `d`, et `e` soient des variables, on peut utiliser les opérateurs plus, moins et multiplier 
avec la notation suivante, et assigner une valeur à `a`:

    int a = 0, b = 1, c = 2, d = 3, e = 4;
    a = b - c + d * e;
    cout << a << endl; // va écrire 1-2+3*4 = 11

Exercise
--------

Dans l'exercice suivant, vous devrez créer un programme qui écrit la somme des nombres `a`, `b`, et `c`.

Tutorial Code
-------------

    #include <iostream>
    using namespace std;

    int main() {
      int a = 3;
      float b = 4.5;
      double c = 5.25;
      double somme;

      /* Votre code ici */

      cout << "La somme de a, b, et c est " << somme << endl;
      return 0;
    }

Expected Output
---------------
    La somme de a, b, et c est 12.75

Solution
--------
    #include <iostream>
    using namespace std;

    int main() {
      int a = 3;
      float b = 4.5;
      double c = 5.25;
      double somme;

      somme = a + b + c;

      cout << "La somme de a, b, et c est " << somme << endl;
      return 0;
    }
