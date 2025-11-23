## 🛠 Résumé du Travail
**Responsabilité : Développement du Cœur Algorithmique**

Dans le cadre de ce projet, ma contribution technique principale a été la conception et l'implémentation robuste des algorithmes d'optimisation en Python, utilisés par l'ensemble du groupe.

**Travaux réalisés :**
1.  **Implémentation du Gradient à Pas Fixe :** J'ai codé l'algorithme itératif $x_{k+1} = x_k - \rho \nabla f(x_k)$. J'y ai intégré des mécanismes de sécurité, notamment une condition d'arrêt sur la norme du gradient ($||\nabla f|| < \epsilon$) et une protection contre les dépassements de capacité (Overflow) pour gérer les fonctions non bornées.
2.  **Implémentation du Gradient à Pas Optimal (Steepest Descent) :** J'ai développé la logique de recherche linéaire. J'ai utilisé la routine `minimize_scalar` de la librairie `scipy.optimize` pour résoudre le sous-problème d'optimisation unidimensionnelle à chaque itération : $\min_{\alpha} f(x_k - \alpha \nabla f(x_k))$.
3.  **Module de Visualisation :** J'ai conçu une fonction de tracé générique (`plot_results`) capable de s'adapter aux différentes topologies étudiées (gestion des échelles logarithmiques pour Rosenbrock, seuillage des valeurs hautes pour Himmelblau), garantissant une uniformité visuelle des résultats du groupe.
