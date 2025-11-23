##  Résumé du Travail
**Responsabilité : Analyse de la Fonction Quadratique (Point Selle)**

Ma contribution technique a consisté à éprouver les limites des algorithmes de descente sur une fonction non convexe et non bornée ($f(x,y) = x^2 - y^2$).

**Analyses et résultats :**
1.  **Démonstration de la Divergence :** J'ai prouvé numériquement l'absence de minimum global. Mes tests montrent une convergence vers 0 sur l'axe convexe ($X$) et une divergence vers $-\infty$ sur l'axe concave ($Y$).
2.  **Gestion de l'Infini :** Face à la croissance exponentielle des valeurs sur l'axe $Y$, j'ai dû paramétrer des conditions d'arrêt strictes (limite de domaine) pour éviter le crash des calculs, illustrant ainsi les risques d'appliquer ces méthodes sur des fonctions non coercives.
3.  **Analyse du Point Selle :** J'ai montré graphiquement que le gradient "fuit" le point stationnaire $(0,0)$ dès l'introduction d'une perturbation infinitésimale (ex: départ à $0.1$), confirmant l'instabilité de ce point critique pour les méthodes de premier ordre.
