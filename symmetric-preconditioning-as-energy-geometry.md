# Symmetric preconditioning as energy geometry

↑ **Parent:** [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md)

For a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $A$, solving $Ax_*=b$ is equivalent to minimizing the [quadratic form](quadratic-form-split.md) with linear term

$$
F(x)=\frac12x^TAx-b^Tx.
$$

Writing the error [vector](vector.md) $e=x-x_*$ and expanding gives the exact [energy norm](energy-norm.md) identity

$$
F(x)-F(x_*)=\frac12e^TAe=\frac12\|e\|_A^2.
$$

The cross term vanishes because $Ax_*=b$. With $\eta=Se$ and $B=S^{-1}AS^{-1}$, the same quantity is $\eta^TB\eta/2$. [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md) changes coordinates without changing the energy assigned to a corresponding error [vector](vector.md).

In an [orthonormal eigenbasis](orthonormal-eigenbasis.md) of $A$, the [level set](level-set.md) $e^TAe=t>0$ has semiaxis lengths $\sqrt{t/\lambda_i}$. Its longest-to-shortest axis ratio is $\sqrt{\kappa_2(A)}$. A large [spectral condition number of a positive-definite matrix](spectral-condition-number-of-a-positive-definite-matrix.md) therefore appears geometrically as a thin [ellipsoid](ellipsoid.md). Good scaling makes the transformed [ellipsoid](ellipsoid.md) rounder, allowing a simple search direction to improve all coordinates together.

The negative [gradient](gradient.md) of $F$ is the [linear-system residual](linear-system-residual.md) $r$. Relative to the [norm](norm.md) $\|v\|_M=\sqrt{v^TMv}$, a steepest direction is $z=M^{-1}r$: the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) applied to $r^Tv=(S^{-1}r)^T(Sv)$ shows that the greatest decrease per unit $M$-length occurs along this direction. Equivalently, ordinary [gradient descent](gradient-descent-split.md) in $y=Sx$ becomes [preconditioned steepest descent](preconditioned-steepest-descent.md) in $x$.[§9.4.1, printed pp. 476–477, equation (9.25), quadratic-norm steepest direction and change of coordinates](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

## ↑ Ancestors (8)

1. [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md)
2. [Matrix preconditioning](matrix-preconditioning.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
