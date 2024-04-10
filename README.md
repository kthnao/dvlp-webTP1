
1.	`npm install` command also generated a package-lock.json file along with package.json. What is the purpose of this file? 
Le fichier package-lock.json sert à enregistrer les versions des dépendances ainsi que leur caractéristiques afin d’assurer que le projet n’ait pas et n’aura de problème de compatibilité au niveau des packages.

2.	By convention, all NPM dependencies use a 3-digit format for version numbers. How do you call this? 
Le format qui utilise les 3 nombres pour désigner une version d’une dépendance s’appelle le Semantic Versioning.

3.	What is a devDependency exactly? What are the differences with a dependency? 
Une devDependency est une dépendance propre à l’environnement de développement et n’est pas utile pour le site web côté utilisateur. Tandis que les ‘dependency’ simples sont nécessaires au bon fonctionnement du site.

4.	What is a closure/iife ? What was it used for ? What replaced it? 
IIFE (Immediately Invoked Function Expression) est une fonnction qui est executé juste après avoir été déclarer. Un closure est une fonction qui se récupérer des informations d’autres fonctions même après qu’elles aient finit de s’exécuter. Cela permet de créer du code séparer du reste pouvant être appelé dans le code global. Cela est remplacé par des imports et des exports. 

5.	What is the difference between import * as toto from './utils' and import { parseUrl } from './utils'? What can be the consequences of using one instead of the other?
Avec *, cela importe toutes les fonctions, qui sont exportées, présentes dans le fichier utils alors que { parseUrl } importe seulement la fonction parseUrl. Utiliser * peut amener à des erreurs ou des confusions si deux méthodes portent le même nom. Tandis qu'utiliser { parseUrl } permettrait une meilleure gestion de la mémoire.

6.	Can you think of at least 2 things that are possible with Java classes, but cannot be done with ES6 classes?
Il n’y a pas d’interface et de méthodes overload avec ES6 classes contrairement aux Java classes. 

7.	What are the differences between var and let
Var est accessible uniquement dans les fonctions lorsqu’on là crée dans la fonction. Lorsqu’elle est créée dans des boucles (while, for, if, …), Var est accessible dans le global scope. Let (pareil pour const) est accessible tout le temps dans la fonction ou boucles et dans les enfants mais pas dans le global scope. 

8.	What is the .bind(this) stuff? What happens if you delete it? Is it needed when using an arrow function ? why ? 
Le .bind(this) permet de lier un contexte à une fonction où le contexte dans ce cas est le this. Si on supprime .bind(this) le contexte de la fonction sera celui avec lequel on a fait appel avec la fonction. La arrow function capture automatiquement le contexte this qui est le contexte de là où elle a été déclarer. Le .bind(this) n ‘est donc pas utile.

9. What does the @ symbol mean in @babel/***? 
Le symbole @ est utilisé pour indiquer un espace de nommage de package dans le gestionnaire de paquets npm.

10. What are the advantages of Promises? 
Les avantages des promesses sont : 
- gestion asynchrone plus simple : permet d'écrire du code de manière séquentielle plutôt que d'utiliser des callbacks imbriqués.
- meilleure lisibilité du code : code plus lisible et plus facile à comprendre en séparant la logique asynchrone de la logique principale du programme.
- meilleure gestion des erreurs :”.catch()” qui permet de capturer les erreurs à n'importe quel niveau de la chaîne de promesses.

11. What version of ECMAScript async / await was released in ? 
L'opérateur async/await a été introduit dans ECMAScript 2017. C'était l'une des fonctionnalités majeures ajoutées à cette version de la spécification ECMAScript. 

12. Component-oriented programming for the web is considered more maintainable. Why? 
La programmation orientée composant pour le web est considérée comme plus maintenable pour sa modularité, sa réutilisabilité, son encapsulation ainsi que sa collaboration.

13. What is Functional programming? 
La programmation fonctionnelle est un paradigme de programmation qui est basée sur l'utilisation de fonctions pour écrire les programmes. Ici, les fonctions peuvent être passées en tant qu'arguments à d'autres fonctions, retournées par d'autres fonctions, et stockées dans des variables. Cela inclue donc l'immuabilité des données (les données ne changent pas une fois qu'elles sont créées), l'évitement des effets secondaires (les fonctions ne modifient pas l'état en dehors de leur portée), et le traitement des programmes comme des évaluations d'expressions mathématiques.

14. Explain what the map() function does ? 
La fonction "map()" est une fonction intégrée utilisée sur les tableaux. Elle permet de transformer chaque élément d'un tableau en appliquant une fonction à chaque élément et en créant un nouveau tableau contenant les résultats de ces transformations. Par exemple, on peut l’utiliser si on a une liste de nombres et que vous voulez tous les multiplier par 2.

15. Explain what the filter() function does ? 
La fonction "filter()" est comme une machine de tri. Elle prend un tas de choses dans un tableau et sélectionne seulement celles qui répondent à certaines règles. Par exemple, si on a une liste de nombres et que vous voulez seulement garder ceux qui sont plus grands que 10, vous pouvez utiliser "filter()". C'est comme avoir une boîte magique qui enlève les choses que vous ne voulez pas garder.

16. Explain what the reduce() function does ? 
La fonction "reduce()"  prend un tas de choses dans un tableau et les combine pour en faire une seule chose. Par exemple, si on a une liste de nombres, on peut les additionner tous ensemble avec "reduce()". C'est comme mettre tous les éléments dans un sac, puis les combiner pour en faire un seul.

17. What is the difference between .then() and async/await when handling asynchronous functions? 
".then()" et "async/await" sont deux façons de gérer les choses qui prennent du temps en JavaScript. ".then()" est comme un ensemble de tâches à faire les unes après les autres, tandis que "async/await" est plus comme faire une pause et une reprise lorsque quelque chose est prêt. C'est comme suivre des étapes étape par étape avec ".then()", alors qu'avec "async/await", c'est comme dire "attends un peu, puis continue".

18. What does the _ prefix mean on a sass file?
Le préfixe “_” dans un fichier Sass signifie que ce fichier est un fichier partiel (fichier contenant des styles CSS réutilisables et qui ne sont pas censés être utilisés directement). Son utilisation permet à Sass de rendre disponible pour l’importation dans d’autres fichiers Sass principaux : il n’est donc pas directement compilé. Cela permet donc à garder les styles bien organisés.
