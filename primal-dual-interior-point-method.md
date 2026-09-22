# Primal-dual interior-point method

↑ **Parent:** [Interior-point method](interior-point-method.md)

A [primal-dual interior-point method](primal-dual-interior-point-method.md) solves perturbed [KKT conditions](karush-kuhn-tucker-conditions.md) while updating both the primal variables and [Lagrange multipliers](lagrange-multiplier.md). For inequalities written as $c_i\geq0$, a logarithmic-barrier path has positive $c_i,y_i$ and perturbed complementarity $c_iy_i=\mu$. A [Newton system](newton-system.md) for these coupled equations gives primal and dual corrections together, with damping to preserve positivity. This can avoid explicitly forming the most ill-conditioned eliminated barrier Hessian, although scaling and regularity still matter.

## ↑ Ancestors (7)

1. [Interior-point method](interior-point-method.md)
2. [Conic optimization](conic-optimization.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/8/v/solution.md)
- [Primal-dual interior-point method](primal-dual-interior-point-method.md)
