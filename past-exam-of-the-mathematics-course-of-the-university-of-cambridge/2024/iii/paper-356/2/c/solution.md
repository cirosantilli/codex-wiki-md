<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The adsorption mechanism is uniform along the two vertical sides, and $X$ evolves independently of $Y$. Consequently the [mean first-passage time](../../../../../../mean-first-passage-time.md) depends only on the initial $x$-coordinate. Its [Kolmogorov backward equation](../../../../../../kolmogorov-backward-equation.md) for $a_1=1$ is

$$
\tau''(x)+\tau'(x)=-1,\qquad -1<x<1.
$$

The forward [partially absorbing boundary condition for a diffusion](../../../../../../partially-absorbing-boundary-condition-for-a-diffusion.md) is $\mathbf J\mathbin\cdot\mathbf n=\kappa p$. The boundary term in the adjoint relation is

$$
\int_{\partial\Omega}
\left(\tau\,\mathbf J\mathbin\cdot\mathbf n
+p\,\partial_n\tau\right)ds,
$$

because the $X$ diffusion coefficient is one. It vanishes for every admissible $p$ precisely when

$$
\partial_n\tau=-\kappa\tau.
$$

For $\kappa=1$, the two [Robin boundary conditions](../../../../../../robin-boundary-condition.md) are therefore

$$
\tau'(-1)=\tau(-1),\qquad
\tau'(1)=-\tau(1).
$$

The general solution of the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) is

$$
\tau(x)=-x+C+De^{-x}.
$$

The right condition gives $C=2$, and the left gives $D=-2/e$. At the prescribed initial position,

$$
\boxed{\tau=\tau(0)=2-\frac2e.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
