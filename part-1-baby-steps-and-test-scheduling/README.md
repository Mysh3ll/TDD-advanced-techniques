Baby steps et ordonnancement des tests
================================================================

**Outils et Techniques Avancés de TDD**

Au-delà des fondamentaux, il existe des techniques et des styles pour progresser dans la pratique du développement piloté par les tests. La première technique est celle des **Petits Pas (Baby Steps)**, déjà évoquée. Puis TDD se décline en deux principaux styles qui peuvent parfois se combiner dans une approche étendue, dite de **Double Boucle**.

Enfin, une autre façon de progresser en TDD consiste à pratiquer sa forme la plus stricte, le **TDD forcé**, ce que l'on pourrait traduire par **"TDD as if you meant it"**.

## Ordonnancement des Tests

La détermination des étapes intermédiaires, c'est-à-dire des cas des tests successifs pour atteindre le résultat final, est un aspect extrêmement important du TDD. Ces étapes doivent être décomposées en petits pas et ordonnées de façon judicieuse.

Il s'agit de décomposer la fonctionnalité en une suite de plusieurs évolutions incrémentales, chacune étant la plus petite possible de manière à ce que cette suite permette d'atteindre la fonctionnalité entière. Une fois cette décomposition en BSP effectuée, ceux-ci sont ordonnés en une séquence progressive qui deviendra la séquence des cas de tests qui vont guider le développement.

Il est donc important de prioriser avec un minimum de connaissances du métier, voire avec une personne représentant le métier. Chaque incrément correspond à un exemple de comportement métier que l'on souhaite supporter. Certains sont extrêmement simples, tels que les cas aux limites, la liste vide, les cas de valeur zéro ou la chaîne vide, tandis que d'autres sont aussi complexes que la fonctionnalité entière.

Dans tous les cas, l'écart entre deux exemples successifs doit rester modeste pour assurer une progression fluide du développement. Si on dessine l'évolution de la fonctionnalité au cours du temps sur un graphe, il s'agit d'avoir un escalier avec de nombreuses petites marches sans aucune grosse marche qui nécessiterait d'implémenter trop de code en un seul incrément.

Puis on énumère les exemples correspondant aux Baby Steps. Dans l'ordre, on commence par écrire un test pour le cas le plus simple, on l'implémente, puis on entame le deuxième exemple et ainsi de suite jusqu'à l'implémentation de tous les Baby Steps de la progression. Il n'est pas rare d'ajouter des cas au cours du développement, par exemple pour décomposer encore plus finement, encore plus de Baby Steps.

Il arrive aussi de changer l'ordre des incréments face à des difficultés inattendues. En effet, un ordonnancement maladroit des Baby Steps peut provoquer une implémentation de complexité inattendue, avec même parfois des impasses.
