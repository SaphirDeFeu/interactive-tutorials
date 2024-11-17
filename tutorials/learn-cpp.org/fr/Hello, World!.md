Tutorial
--------

### Introduction

C++ (prononcé sé-plus-plus) est une langue de programmation à usage généralisé qui est à forme libre et compilé. Il est vu comme une langue de niveau intermédiaire, car il comprend à la fois des caractéristiques de langue haut-niveau et bas-niveau. Il fournit des fonctionnalités de programmation impératives, orientées objet et génériques.

C++ est l'une des plus populaires langues de programmation et est implémenté dans une grande variété de plateformes de système d'exploitation ou matérielle. En tant que langue de programmation axée sur la performance, elle est utilisé dans les logiciels systèmes, les applications, les pilotes d'appareils, logiciels intégrés, serveurs à haute-performance et applications clients, et des logiciels de divertissement tel que les jeux vidéos. Diverses entités propose à la fois des logiciels de compilation C++ source-ouverte et source-fermée, dont la FSF, LLVM, Microsoft et Intel.

### Notre premier programme

Chaque programme C++ fait appel à des librairies, qui nous donnent la possibilité d'exécuter des fonctions nécessaires. Par exemple, la fonction la plus basique
appelée 'cout', qui écrit à l'écran, est définie dans le fichier d'en-tête `iostream`. 

Pour ajouter la possibilité d'exécuter la commande `cout` à notre programme, nous devons ajouter la directive include suivante à notre première ligne de code:

    #include <iostream>
    using namespace std;

La deuxième partie du code est le véritable code que nous allons écrire. Le tout premier code qui va être exécuté réside toujours 
dans la fonction `main`. 

    int main() {
      ... notre code va ici
    }

Le mot-clé `int` indique que la fonction `main` retourne un entier - un simple nombre. Le nombre retourné
par la fonction indique si le program que nous avons écrit fonctionne correctement. Si on veut dire que notre code
a été exécuté correctement, nous retournons le nombre 0. Un nombre supérieur à 0 signifie que le programme que nous avons écrit a échoué.

Pour ce tutoriel, nous retournerons 0 pour indiquer que notre programme était un succès:

    return 0;

Remarquez que chaque ligne en C++ doit se terminer par un point-virgule, de manière à ce que le compilateur sache quand une nouvelle ligne commence.

Enfin, nous devrons utiliser une redirection au flux `cout` pour écrire notre phrase.

Exercise
--------

Changez le programme en bas de manière à ce qu'il écrive "Hello, world!" dans la console. 

Tutorial Code
-------------

    #include <iostream>
    using namespace std;

    int main() {
      cout << "Goodbye, World!" << std::endl;
      return 0;
    }

Expected Output
---------------

    Hello, World!

Solution
--------

    #include <iostream>
    using namespace std;

    int main() {
      cout << "Hello, World!" << std::endl;
      return 0;
    }
