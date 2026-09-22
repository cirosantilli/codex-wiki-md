# Residual and forward error in a stationary iteration

↑ **Parent:** [Iteration matrix](iteration-matrix.md)

The [linear-system residual](linear-system-residual.md) $r^{(k)}=b-Ax^{(k)}$ is computable without knowing $x_*$. The [forward error](forward-error.md) $e^{(k)}=x^{(k)}-x_*$ is the actual difference from the desired solution. For an [invertible matrix](invertible-matrix.md),

$$
r^{(k)}=-Ae^{(k)},\qquad e^{(k)}=-A^{-1}r^{(k)}.
$$

Keeping $A$ fixed, the approximate [vector](vector.md) exactly solves $Ax^{(k)}=b+\delta b$ with $\delta b=-r^{(k)}$. Thus, for $b\ne0$, $\|r^{(k)}\|/\|b\|$ is the relative [backward error](backward-error.md) when only the right-hand side may change. For a [vector norm](norm.md) and its induced [operator norm](operator-norm.md),

$$
\frac{\|e^{(k)}\|}{\|x_*\|}\leq\kappa(A)\frac{\|r^{(k)}\|}{\|b\|},\qquad \kappa(A)=\|A\|\,\|A^{-1}\|.
$$

A small relative [linear-system residual](linear-system-residual.md) ensures a small relative [forward error](forward-error.md) when the [condition number](condition-number.md) is moderate; an ill-conditioned [matrix](matrix.md) can amplify it. The bound follows directly from $e=-A^{-1}r$ and $\|b\|=\|Ax_*\|\leq\|A\|\|x_*\|$.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §2.8.1, Theorem 2.8.1, equation (2.8.6), right-hand-side perturbation bound applied with Δb = −r](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/2-8-conditioning-of-linear-systems.md)

For the [Jacobi iteration for a three-variable tridiagonal system](jacobi-iteration-for-a-three-variable-tridiagonal-system.md), the first [linear-system residual](linear-system-residual.md) is $(1,3,1)^T$, while the first [forward error](forward-error.md) is $(-1/2,-1,-1/2)^T$. In the [Euclidean norm](euclidean-norm.md), the relative [forward error](forward-error.md) is $\sqrt{3/28}\approx0.3273$ and the relative [linear-system residual](linear-system-residual.md) is $\sqrt{11/120}\approx0.3028$. Its [spectral condition number of a positive-definite matrix](spectral-condition-number-of-a-positive-definite-matrix.md) is $(4+\sqrt2)/(4-\sqrt2)\approx2.094$, so the bound is about $0.6340$. The bound is a guarantee, not an equality. In [floating-point arithmetic](floating-point-arithmetic-split.md), recompute the [linear-system residual](linear-system-residual.md) from the current [vector](vector.md) when checking termination; a small update alone need not certify a small [forward error](forward-error.md).

## ↑ Ancestors (8)

1. [Iteration matrix](iteration-matrix.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Error modes of a three-variable Jacobi iteration](error-modes-of-a-three-variable-jacobi-iteration.md)
