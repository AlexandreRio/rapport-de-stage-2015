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
* Runtime bien trop lourd (de l'ordre de 300k), sans compter le parser en lui même.

## Lundi 29
Essayer de modifier du code généré par Flex et Bison pour Coffee, le FS de Contiki
Erreur au moment de linker après modifications du chargement du buffer depuis le disque, `__libc_fini_array`

## Mardi 30
Custom solution from scratch, limites de mémoire en allocation dynamique pour les tokens du lexer

## Mercredi 01
idée de partir du json-parser de contiki pour le faire détecter les types d'objets courants et créer les instances

## Jeudi 02
Changement de projet, le parser spécifique est très galère. Génération du code C depuis le méta-modèle. Une première version est déjà faite pour une ancienne version de Kevoree, l'idée est d'automatiser la génération des classes et de la lib (recherche de nœud, visite, comparaison, séréalisation)

Et j'ai 15jours de blanc dans mes notes… Il reste plus qu'à aller voir mon historique de commits…