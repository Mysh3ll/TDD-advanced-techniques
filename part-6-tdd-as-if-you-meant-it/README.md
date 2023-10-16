TDD as if you meant it
================================================================

## La rigueur du TDD et "As If You Meant It" (Comme si vous le vouliez)

L'idée derrière la pratique _stricte_ du Test-Driven Development (**TDD**) est de pousser cette méthode au maximum avec l'approche "**_TDD As If You Meant It_**". Cette approche exige de retenir ses réflexes d'implémentation habituels. En d'autres termes, on commence par mettre tout le code, y compris celui qui est destiné à être livré en production à terme, dans le corps de la méthode de test.

Bien que cela puisse sembler contre-intuitif au départ, l'objectif est de progresser avec le code strictement nécessaire, rassemblé en un seul endroit pour pouvoir tout visualiser aisément. La seule façon d'introduire une méthode, une classe, ou même une constante est de le faire par "_factoring_" à partir du code déjà fonctionnel dans la méthode de test.

L'approche "**_TDD As If You Meant It_**" consiste à éviter de concevoir les classes et les interfaces des méthodes dès le début, afin de laisser le **TDD** faire émerger la conception sans être influencé par nos anticipations. Lorsque l'on débute un cycle de **TDD**, le code subit un "_factoring_" à un rythme rapide, généralement de l'ordre de quelques secondes ou minutes. Avoir tout le code dans une même méthode ou un même fichier facilite ce processus.

Au fil du développement et des tests, le code a tendance à croître et à changer un peu moins radicalement. C'est alors le moment d'extraire les éléments de conception de plus en plus englobants, tels que les méthodes, les classes, et éventuellement les modules, qui formeront progressivement la structure du code.

Introduire des éléments de conception tels que les packages, les classes et les méthodes qui rendent le code plus difficile à changer survient au moment le plus opportun, c'est-à-dire lorsque le code a déjà prouvé son fonctionnement après avoir passé plusieurs tests. La démarche consiste à ne pas penser au design de la solution et à y aller vraiment sans idée préconçue.

Bien que cela puisse sembler simple, inconsciemment, on cherche souvent à trouver le meilleur design avant même de décomposer le problème. Avec l'expérience, il est courant de reproduire des solutions passées considérées comme des modèles à suivre ou d'éviter des erreurs passées. Cependant, l'essence même du **TDD** pur est d'ouvrir la voie à de nouvelles propositions de solutions, tout en tenant compte des expériences passées.
