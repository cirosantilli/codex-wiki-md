<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Gram matrix](../../../../../../gram-matrix.md) representation and $Y_{ii}=1$ give $\|v_i\|_2=1$. For a [standard Gaussian random vector](../../../../../../standard-gaussian-random-vector.md) $Z$, each $\langle v_i,Z\rangle$ is a standard [normal](../../../../../../normal-distribution.md) [scalar](../../../../../../scalar.md), so the zero event has [probability](../../../../../../probability.md) zero. Choose either sign convention at zero; the resulting [vector](../../../../../../vector.md) is [almost surely](../../../../../../almost-sure-convergence.md) a feasible sign [vector](../../../../../../vector.md). Consequently $y^TAy\leq v^*$ [almost surely](../../../../../../almost-sure-convergence.md).

The [Gaussian sign-correlation identity](../../../../../../gaussian-sign-correlation-identity.md) gives

$$
\mathbb E[y^TAy]
=\sum_{i,j}A_{ij}\mathbb E[y_iy_j]
=\frac2\pi\sum_{i,j}A_{ij}\arcsin(Y_{ij})
=\frac2\pi\operatorname{tr}(A\arcsin[Y]).
$$

The last equality uses symmetry of the real [matrices](../../../../../../matrix.md). Hence

$$
\boxed{v^*\geq\mathbb E[y^TAy]
=\frac2\pi\operatorname{tr}(A\arcsin[Y])}.
$$

The [inverse sine](../../../../../../inverse-sine.md) is applied entrywise, not through [spectral matrix functional calculus](../../../../../../spectral-matrix-functional-calculus.md).

For completeness, the [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) identity has a geometric proof. If the angle between two unit [vectors](../../../../../../vector.md) is $\theta$, the isotropic [Gaussian random vector](../../../../../../gaussian-random-vector.md) direction in their two-dimensional span gives opposite signs on angular sectors with [probability](../../../../../../probability.md) $\theta/\pi$. Thus the sign product has [expectation](../../../../../../expected-value.md) $1-2\theta/\pi=(2/\pi)\arcsin(\cos\theta)$. Parallel and antiparallel pairs give the endpoint values $1$ and $-1$ directly. This is [Gaussian hyperplane rounding](../../../../../../gaussian-hyperplane-rounding.md), and needs no [independence](../../../../../../independent-random-variables.md) between the rounded coordinates.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
