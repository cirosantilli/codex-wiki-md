<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [objective function](../../../../../../objective-function.md) $\theta$ is nonnegative. We now construct a feasible zero-objective point, distinguishing the input problem's possible states.

If the primal is feasible and bounded below, [strong duality](../../../../../../strong-duality.md) and attainment for a [linear program](../../../../../../linear-programming.md) give $x_*\ge0$, $\lambda_*$ and $s_*=c-A^T\lambda_*\ge0$ with

$$
Ax_*=b,\qquad c^Tx_*=b^T\lambda_*.
$$

Set $\theta=\kappa=0$, $\tau=1$, $x=x_*$, $s=s_*$, $\lambda=\lambda_*$, and

$$
\rho=\frac{e^Tx_*+e^Ts_*+1}{N}>0.
$$

The first three embedding equations hold. Substituting their equalities into the fourth gives precisely $-e^Tx_*-e^Ts_*-1+N\rho=0$.

If the primal is infeasible, the [Farkas alternative](../../../../../../farkas-lemma.md) supplies $\lambda$ with $A^T\lambda\le0$ and $b^T\lambda>0$. Take $x=\tau=\theta=0$, $s=-A^T\lambda\ge0$, $\kappa=b^T\lambda>0$, and $\rho=(e^Ts+\kappa)/N$. These satisfy the same equations. If the primal is feasible and unbounded below, it has a direction in the [recession cone](../../../../../../recession-cone.md) $x\ge0$ with $Ax=0$ and $c^Tx<0$. Set $\lambda=s=\tau=\theta=0$, $\kappa=-c^Tx>0$, and $\rho=(e^Tx+\kappa)/N$. This is again a feasible nonzero embedding [vector](../../../../../../vector.md). Normalize the constructed [vector](../../../../../../vector.md) by the sum of its nonnegative coordinates. In every case,

$$
\boxed{\min c^{*T}y=\min\theta=0.}
$$

The facts about optimal pairs and recession directions follow from the polyhedral alternatives of [linear programming duality](../../../../../../linear-programming-duality.md); they do not require knowing their values or witnesses to write the transformed coefficients.

To recover information from the transformed optimum, multiply the first three original embedding equations by $\lambda^T$, $x^T$, and $\tau$, respectively, and add. Their cross terms cancel; the fourth equation gives

$$
x^Ts+\tau\kappa=N\theta\rho.
$$

At $\theta=0$, nonnegativity forces $x^Ts=0$ and $\tau\kappa=0$. The equations also imply

$$
e^Tx+e^Ts+\tau+\kappa=N\rho.
$$

Thus any normalized zero-objective point has $\rho>0$: if $\rho=0$, all these coordinates vanish, and then $q=\lambda=\theta=0$, contradicting normalization.

If $\tau>0$, division by $\tau$ gives a primal-feasible point $x/\tau$ and dual-feasible point $\lambda/\tau$ with equal [objective function](../../../../../../objective-function.md) values; hence they are optimal. If $\kappa>0$, then $\tau=0$, $Ax=0$, $A^T\lambda=-s\le0$, and

$$
b^T\lambda-c^Tx=\kappa>0.
$$

Therefore either $b^T\lambda>0$ certifies primal infeasibility, or $c^Tx<0$ is an improving recession direction certifying dual infeasibility and unboundedness whenever the primal is feasible. If only the latter certificate is obtained and primal feasibility is unknown, apply the same construction to the feasibility problem with [objective function](../../../../../../objective-function.md) $c=0$; it gives either a [feasible point](../../../../../../feasible-point.md) or a direct primal infeasibility certificate.

A degenerate optimal point can have $\tau=\kappa=0$ and convey neither conclusion. Choose an optimum in the [relative interior](../../../../../../relative-interior.md) of the [optimal face of a linear program](../../../../../../optimal-face-of-a-linear-program.md). The explicit existence argument above gives a point of this face with $\tau+\kappa>0$. A nonnegative coordinate which is positive somewhere on a [face of a convex set](../../../../../../face-of-a-convex-set.md) is positive throughout its [relative interior](../../../../../../relative-interior.md), so the chosen point has $\tau+\kappa>0$ and can be decoded. The assertion follows because a small relative-interior displacement in the direction opposite a positive-coordinate point would otherwise make that coordinate negative. Equivalently one may obtain a maximum-support optimum; choosing an arbitrary degenerate boundary optimum is insufficient.

This reduction is useful because an [interior-point method](../../../../../../interior-point-method.md) now has a known strictly feasible start, a compact [standard simplex](../../../../../../standard-simplex.md) slice, and a known target [objective function](../../../../../../objective-function.md). Projective rescalings can recenter positive iterates, and the transformed problem supplies optimality or infeasibility information without a separate guessed optimum. Polynomial bit-complexity claims need rational data with a finite encoding length. The printed bound $U$ on arbitrary real coefficients by itself does not bound denominators or the size of nonzero [determinants](../../../../../../determinant.md); it is not a substitute for that encoding assumption.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
