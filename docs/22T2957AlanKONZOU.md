## 📉 Résumé du Travail
**Responsabilité : Analyse de la Fonction de Rosenbrock**

Mon travail a porté sur l'étude comportementale des algorithmes face à une fonction mal conditionnée ("La Banane de Rosenbrock").

**Analyses et résultats :**
1.  **Instabilité du Pas Fixe :** J'ai démontré empiriquement la grande sensibilité de cet algorithme à la courbure de la vallée. J'ai déterminé qu'un pas $\rho > 0.002$ provoquait une divergence immédiate, et j'ai calibré le paramètre $\rho = 0.002$ pour assurer une convergence lente mais stable.
2.  **Phénomène de Zig-Zag :** J'ai mis en évidence le comportement caractéristique de la méthode du pas optimal (Steepest Descent). Les graphiques produits montrent que les directions successives de descente sont orthogonales, ce qui entraîne de nombreuses petites itérations pour progresser au fond de la vallée étroite.
3.  **Visualisation Logarithmique :** Pour valider l'atteinte du minimum en $(1,1)$, j'ai configuré l'affichage des lignes de niveau avec une échelle logarithmique (`LogNorm`), seule méthode permettant de distinguer la topologie du fond de la vallée.
