## Résumé du Travail
**Responsabilité : Analyse de la Fonction de Himmelblau**

J'ai exploré la problématique de la multimodalité (minima multiples) pour vérifier le déterminisme local des algorithmes de gradient.

**Analyses et résultats :**
1.  **Cartographie des Bassins d'Attraction :** J'ai mis en place une stratégie de tests systématiques en variant les points initiaux $x_0$ dans les quatre quadrants du plan.
2.  **Validation des 4 Minima :** J'ai réussi à faire converger l'algorithme vers les quatre solutions globales distinctes connues : $(3,2)$, $(-2.8, 3.1)$, $(-3.7, -3.2)$ et $(3.5, -1.8)$, prouvant que le résultat final dépend entièrement des conditions initiales.
3.  **Visualisation Topographique Avancée :** J'ai affiné la représentation graphique en appliquant une coupe sur l'axe Z (valeurs $> 200$ ignorées). Cela a permis de faire apparaître visuellement les quatre "cuvettes" bleues simultanément et de tracer les trajectoires de descente plongeant dans chacune d'elles.
