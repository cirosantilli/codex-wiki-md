<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A reduction must encode primal solutions and infeasibility or unboundedness information; merely declaring a known optimum or subtracting an unknown optimum from the [objective function](../../../../../objective-function.md) is not a construction. The following [homogeneous self-dual embedding of a linear program](../../../../../homogeneous-self-dual-embedding-of-a-linear-program.md) works without assuming the input problem has an optimum.

First remove linearly dependent equality rows by [Gaussian elimination](../../../../../gaussian-elimination.md). If an eliminated row has an inconsistent right-hand side, the original problem is already certified infeasible. Return the one-variable special-form program $\min 0$ with $A^*=0$, $y=1$, and retain that certificate; no original [mathematical optimization](../../../../../mathematical-optimization-split.md) remains. Otherwise the remaining [matrix](../../../../../matrix.md) has [full row rank](../../../../../full-row-rank.md); write it as $A$ again. Put $e=\mathbf1\in\mathbb R^n$ and

$$
\bar b=b-Ae,\qquad \bar c=c-e,\qquad \bar z=c^Te+1,\qquad N=n+1.
$$

Use nonnegative variables $x,s\in\mathbb R^n$ and $\tau,\kappa,\theta,\rho\in\mathbb R$, with a temporary unrestricted multiplier $\lambda\in\mathbb R^m$. Impose the [homogeneous linear system](../../../../../homogeneous-linear-system.md)

$$
\begin{aligned}
Ax-b\tau+\bar b\theta&=0,\\
-A^T\lambda+c\tau-s-\bar c\theta&=0,\\
b^T\lambda-c^Tx-\kappa+\bar z\theta&=0,\\
-\bar b^T\lambda+\bar c^Tx-\bar z\tau+N\rho&=0.
\end{aligned}
$$

All coefficients are computable from the input. The temporary free multiplier can be eliminated without introducing cancelling positive/negative variables. Define

$$
H=(AA^T)^{-1}A,\quad q=c\tau-s-\bar c\theta,\quad
\lambda=Hq.
$$

Replace the second equation by $(I-A^TH)q=0$, and substitute $Hq$ in the other equations. Because $A$ has [full row rank](../../../../../full-row-rank.md), $A^T\lambda=q$ is equivalent to these conditions. For no remaining equality rows, simply omit $\lambda$ and its empty equations.

Let $y=(x,s,\tau,\kappa,\theta,\rho)$ and $n^*=2n+4$. Collect these substituted equations into $A^*y=0$, impose $\mathbf1^Ty=1$, and let $c^*$ select the coordinate $\theta$. The resulting [Karmarkar standard form](../../../../../karmarkar-standard-form.md) is

$$
\boxed{\min\theta,\qquad A^*y=0,\quad\mathbf1^Ty=1,\quad y\ge0.}
$$

The next two parts prove its known positive starting point and zero optimal value. Notice that normalization is legitimate for any nonzero nonnegative embedding [vector](../../../../../vector.md) because all the equations are homogeneous; it does not require a prior bound on the original optimizer.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
