# Descente_de_Gradient
Expérimentation des descentes de gradients à pas fixe et à pas optimal 
# TP d'Optimisation II : Algorithmes de Descente
**Cours :** INF4127 - Optimisation II
**Université :** Université de Yaoundé 1
**Date :** Novembre 2025

---

## 🎯 Objectif du Projet
Ce projet vise à implémenter et analyser le comportement de deux algorithmes d'optimisation sans contraintes sur trois fonctions tests classiques. L'objectif est de comprendre l'influence du **pas de descente** ($\rho$) et de la **géométrie de la fonction** sur la convergence.

## 📐 Rappels Théoriques

Nous cherchons à résoudre : $\min_{x \in \mathbb{R}^n} f(x)$.

### 1. Algorithme du Gradient à Pas Fixe
C'est la méthode la plus simple. On se déplace dans la direction opposée au gradient avec un pas constant $\rho$.
$$x_{k+1} = x_k - \rho \nabla f(x_k)$$
* **Avantage :** Simple à coder.
* **Inconvénient :** Le choix de $\rho$ est critique (trop petit = lent, trop grand = divergence).

### 2. Algorithme du Gradient à Pas Optimal (Steepest Descent)
À chaque itération, on cherche le meilleur pas $s_k$ qui minimise la fonction dans la direction de descente $d_k = -\nabla f(x_k)$.
$$s_k = \arg \min_{s > 0} f(x_k + s d_k)$$
$$x_{k+1} = x_k + s_k d_k$$
* **Avantage :** Convergence garantie à chaque étape.
* **Inconvénient :** Coûteux en calcul et peut faire des "zig-zags" dans les vallées étroites.

## 📂 Structure du Dépôt
Le travail est divisé en trois analyses indépendantes :

| Fichier | Fonction Étudiée | Particularité 
| :--- | :--- | :--- | 
| `1_Rosenbrock.ipynb` | Rosenbrock | Vallée étroite (Conditionnement difficile) 
| `2_Quadratique.ipynb` | Quadratique | Point Selle (Non convexe) 
| `3_Himmelblau.ipynb` | Himmelblau | Multi-modalité (4 minima) 

## 🚀 Installation et Exécution
Pour lancer les notebooks, assurez-vous d'avoir les librairies suivantes :
```bash
pip install numpy matplotlib pandas scipy
