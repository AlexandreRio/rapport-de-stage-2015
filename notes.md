# Semaine 1

Comparaison des algos

## Lundi 01 Juin

Matin:

* problème de migration de l'annuaire,
* badge,
* lecture du papier Towards a Model@Runtime Middleware

Après-midi:

* description du problème de compression,
* mise en place de l'env de dev,
* rapide coup d'œil aux mots clés d'un fichier de modèle


# Semaine 2

Implémentation de la compression par table association sur contiki,
tests de portage des autres algos,

## Jeudi 11

Coffee de présentation informel, ~5min, en anglais

# Semaine 3

* Expé de dissémination de modèle compressé
* explications du parser du meta-modèle vers kevoree-c
* correction du bug de décompression après dissémination

# Semaine 4

LLVM, flex bison, antlrv3
Parser de fichier de modèles

## Mercredi 24/Jeudi 25
séminaire d'équipe

## Vendredi 26
AntlrV3, peut produire un parser en C

Pros:
* Déjà utilisé en cours

Cons:
* Runtime bien trop lourd (de l'ordre de 300kb), sans compter le parser en lui même.

## Lundi 29
Essayer de modifier du code généré par Flex et Bison pour Coffee, le FS de Contiki
Erreur au moment de linker après modifications du chargement du buffer depuis le disque, `__libc_fini_array`

## Mardi 30
Custom solution from scratch, limites de mémoire en allocation dynamique pour les tokens du lexer

## Mercredi 01
idée de partir du json-parser de contiki pour le faire détecter les types d'objets courants et créer les instances

## Jeudi 02
Changement de projet, le parser spécifique est très galère. Génération du code C depuis le méta-modèle. Une première version est déjà faite pour une ancienne version de Kevoree, l'idée est d'automatiser la génération des classes et de la lib (recherche de nœud, visite, comparaison, séréalisation)

# Semaine X

## Jeudi 09
Réunion informelle avec O. Ridoux pour discuter compilateurs et génération de code ainsi que de la structure d'un parser optimisé.

# Semaine X+1

## Mercredi 15
Réunion avec F. Fouquet sur l'avenir de KMF, les changements introduit par la dernière version.
Lecture de deux papiers non publiés pour le moment.

## Jeudi 16
Compilation sans erreur des sources générées (nombreux warnings déjà présents dans la version utilisée venant de cast de pointeur)

Écrire d'un "test" simple de création d'instance, les pointeurs de fonction sont initialisé à la main dans le code généré puisqu'ils ne sont pas générés. La structure actuelle du générateur de code rendrait trop pénible leur ajout et trop difficilement maintenable.

## Vendredi 17
Début de refactoring du générateur, idée d'arriver à une meilleure représentation interne, plus proche du langage intermédiaire des compilateurs.


Et j'ai 15jours de blanc dans mes notes… Il reste plus qu'à aller voir mon historique de commits…
