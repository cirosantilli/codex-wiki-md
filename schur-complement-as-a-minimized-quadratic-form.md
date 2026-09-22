# Schur complement as a minimized quadratic form

↑ **Parent:** [Schur complement](schur-complement.md)

Let $M=\begin{pmatrix}A&B\\B^T&D\end{pmatrix}$ be a real [symmetric matrix](symmetric-matrix.md) with $A$ a [positive-definite matrix](positive-definite-matrix.md). Its [quadratic form](quadratic-form-split.md) satisfies the [completing the square](completing-the-square.md) identity

$$
q(x,y)=x^TAx+2x^TBy+y^TDy
=(x+A^{-1}By)^TA(x+A^{-1}By)+y^T(D-B^TA^{-1}B)y.
$$

For each fixed [vector](vector.md) $y$, the unique minimizing [vector](vector.md) is $x=-A^{-1}By$, so the minimized value is $y^TSy$. Also, $M$ is a [positive-definite matrix](positive-definite-matrix.md) exactly when $S$ is a [positive-definite matrix](positive-definite-matrix.md), under the stated assumption on $A$.[Appendix A.5.5, printed p. 650, equations (A.13)–(A.14) and the following definiteness criteria](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

An original scalar example is

$$
q(x,y)=2x^2+2xy+3y^2=2(x+y/2)^2+\frac52y^2.
$$

Here $A=2$, $B=1$, $D=3$, and the [Schur complement](schur-complement.md) is $5/2$. Holding $x=0$ would give $3y^2$, but letting $x$ relax to $-y/2$ reduces the [quadratic form](quadratic-form-split.md) to $(5/2)y^2$. At $y=2$ the respective values are $12$ and $10$. Eliminating a variable therefore changes the effective cost of the retained variable.

<a id="image-a-schur-complement-measures-the-quadratic-form-left-after-another-variable-relaxes"></a>
![](schur-complement-quadratic-relaxation.png)

**[Figure 27](#image-a-schur-complement-measures-the-quadratic-form-left-after-another-variable-relaxes). A Schur complement measures the quadratic form left after another variable relaxes**. Original contours of $q(x,y)=2x^2+2xy+3y^2$ and the two resulting costs. The minimizing line $x=-y/2$ picks the least value at each fixed $y$; the plotted profiles are exact model values, not experimental measurements.

This interpretation supports [quadratic optimization](quadratic-optimization.md) and the [positive-definite symmetric matrix](symmetric-positive-definite-matrix.md) tests used in [Cholesky decomposition](cholesky-decomposition.md). In a [multivariate normal distribution](multivariate-normal-distribution.md), a [covariance matrix](covariance-matrix.md) also gives a [conditional covariance](conditional-covariance.md) through a [Schur complement](schur-complement.md); the required probabilistic hypotheses are supplied by [conditional multivariate normal distribution](conditional-multivariate-normal-distribution.md), rather than by the algebra alone.

## ↑ Ancestors (6)

1. [Schur complement](schur-complement.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Schur complement](schur-complement.md)
