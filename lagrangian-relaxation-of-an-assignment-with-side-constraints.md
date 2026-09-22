# Lagrangian relaxation of an assignment with side constraints

↑ **Parent:** [Lagrangian relaxation](lagrangian-relaxation.md)

Retaining [integer](integer-split.md) assignment equations while dualizing extra capacity inequalities gives an easily evaluated [upper bound](upper-bound-in-a-partially-ordered-set.md) for a maximization problem. With multipliers $\lambda\geq0$ and capacities $b$, it is $\theta(\lambda)=\max_{x\text{ assignment}}[c^Tx+\lambda^T(b-Ax)]$. It is a convex maximum of affine functions. Minimizing it exploits the [convex hull](convex-hull.md) of assignments, so it can have a finite optimum when only a fractional mixture satisfies the side constraints and no [integer](integer-split.md) assignment does. This separates a useful relaxation bound from a certificate of [integer](integer-split.md) feasibility.

## ↑ Ancestors (8)

1. [Lagrangian relaxation](lagrangian-relaxation.md)
2. [Lagrangian dual problem](lagrangian-dual-problem.md)
3. [Linear programming duality](linear-programming-duality.md)
4. [Linear programming](linear-programming-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2010/3/a/solution.md)
