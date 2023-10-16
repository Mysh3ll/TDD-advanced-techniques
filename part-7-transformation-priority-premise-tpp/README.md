Transformation Priority Premise (TPP)
================================================================

En appliquant le **TDD** (Test Driven Development), nous enrichissons le code de production au fur et à mesure des ajouts de nouveaux tests. Lors de la phase de factoring dans le cycle du TDD (_Rouge, Vert, Factoring ou Red-Green_), nous améliorons la lisibilité du code en changeant sa structure sans modifier son comportement.

Robert C. Martin, dans son [blog](https://blog.cleancoder.com/uncle-bob/2013/05/27/TheTransformationPriorityPremise.html), propose des 
transformations priorisées, connues sous le nom de Transformation Priority Premise (TPP), pour rester fidèle au principe des _baby steps_. Les transformations consistent en des modifications de code simples qui changent le comportement, tout en maintenant la structure aussi simple que possible.

Voici la liste des transformations déterminées par Robert C. Martin :

- `{} -> null`: Partir sans code vers un code qui emploie ou retourne null
- `null -> constante`: Transformer le null en utilisant une constante
- `constante -> constante+`: Transformer une constante simple en une constante plus complexe
- `constante -> scalaire`: Remplacer une constante par une variable ou un argument
- `instruction -> instructions`: Ajouter des instructions sans condition
- `unconditionel -> If`: Introduire une condition
- `scalaire -> tableau`
- `tableau -> conteneur`
- `Instruction -> Récursion`
- `if -> while`
- `expression -> Fonction`: Remplacer une expression par une fonction ou un algorithme
- `variable -> affectation`

Ces transformations, allant du spécifique au générique, peuvent être appliquées dans l'exercice du kata _FizzBuzz_. En respectant l'ordre des priorités des transformations, on évite de sauter trop rapidement vers un code complexe et superflu, ce qui est crucial dans la pratique du **TDD**.

Il est essentiel de garder à l'esprit ces principes lors de l'application du **TPP**.
