Remerciements
==

Remercier l'IRISA pour sa structure, DiverSE pour son accueil, Johann, Paco et Inti.

Intro
==

Mon stage d'ESIR2, à la frontière entre l'embarqué et le SE.

Sert d'introduction à mon année de double cursus ESIR/MRI.

Concept de model@runtime

Partie 1
==

Environnement Contiki
--

* limites du système (débug, compilation, runtime C),
* limites des nœuds (caractéristiques physiques, topologie du réseau),

Testbed iot-lab
--

* utilité,
* structure (différents lieux (Roquencourt \o/), types de nœud),
* utilisation (web ui ou cli, experiment)

Kevoree
--

Expliquer ce qu'est kevoree… Sans trop rentrer dans les détails ou dans les aspects trop éloignés de mon stage. Éviter de parler d'implémentation.

Partie 2
==

Partie sur le travail réalisé,

compression des modèles
--

étude de l'art, contraintes systèmes, algo à la mano

table des perfs mesurées, outils utilisés, truc propre quoi (pour compensé l'algo bencale)

parser spécifique
--

vu le fiasco on va pas s'étendre…

Expliquer qu'il vaut mieux générer les «classes» puis générer un parser générique, ce sera aussi compliqué mais plus rapide que faire `spécifique -> générique`

générateur de code depuis le méta-modèle
--

le sujet principal du stage, ça parle de compilation donc c'est cool.

détailler les points communs entre ce genre de projet et un compilateur «classique».
