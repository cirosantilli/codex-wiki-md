# Homogeneous self-dual embedding of a linear program

↑ **Parent:** [Interior-point method](interior-point-method.md)

For a [linear program](linear-programming.md) $\min\{c^Tx:Ax=b,\ x\ge0\}$ and its [dual linear program](dual-linear-program.md), write $e=\mathbf1$, $\bar b=b-Ae$, $\bar c=c-e$, and $\bar z=c^Te+1$. Introduce $x,s\ge0$, $\tau,\kappa,\theta,\rho\ge0$, and a free multiplier $\lambda$ satisfying

$$
Ax-b\tau+\bar b\theta=0,\quad
-A^T\lambda+c\tau-s-\bar c\theta=0,\quad
b^T\lambda-c^Tx-\kappa+\bar z\theta=0,\quad
-\bar b^T\lambda+\bar c^Tx-\bar z\tau+(n+1)\rho=0.
$$

The point $x=s=e$, $\tau=\kappa=\theta=\rho=1$, $\lambda=0$ is strictly positive in all constrained coordinates. Multiplying the first three equations by $\lambda^T,x^T,\tau$ respectively and adding gives the displayed identity. Minimizing $\theta$ has value zero: primal-dual optimal solutions or certificates from [Farkas' lemma](farkas-lemma.md) give zero-$\theta$ solutions after selecting positive $\rho$ and scaling. At $\theta=0$, $\tau>0$ gives an optimal primal-dual pair by division by $\tau$, while $\kappa>0$ gives a primal infeasibility or dual infeasibility certificate. A point with $\tau=\kappa=0$ is not decisive; choosing a [relative interior](relative-interior.md) point of the [optimal face of a linear program](optimal-face-of-a-linear-program.md) avoids that degeneracy because the face contains a point with $\tau+\kappa>0$.

## ↑ Ancestors (7)

1. [Interior-point method](interior-point-method.md)
2. [Conic optimization](conic-optimization.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Karmarkar standard form](karmarkar-standard-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/3/solution.md)
