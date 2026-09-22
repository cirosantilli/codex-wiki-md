<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed weights during the input average,

$$
\langle yx\rangle=\langle xx^T\rangle w=Cw,\qquad
\langle y^2\rangle=w^TCw.
$$

Thus $C$ is the input second-moment matrix. It is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) because $v^TCv=\langle(v^Tx)^2\rangle\geq0$. If the inputs have been mean-centered, it is their [covariance matrix](../../../../../../covariance-matrix.md); otherwise $C=\operatorname{Cov}(x)+\langle x\rangle\langle x\rangle^T$.

The stationary averaged learning equation is

$$
\boxed{Cw=\alpha\langle y^2\rangle w.}
$$

For $w\ne0$ this makes $w$ an [eigenvector](../../../../../../eigenvector.md) of $C$ with [eigenvalue](../../../../../../eigenvalue.md) $\lambda=\alpha\langle y^2\rangle$. If $\lambda>0$, taking the inner product with $w$ gives

$$
\lambda\|w\|^2=\alpha(w^TCw)\|w\|^2,
\qquad w^TCw=\lambda\|w\|^2,
$$

and therefore

$$
\boxed{\|w\|^2=1/\alpha.}
$$

The zero vector is also stationary but is not an eigenvector in the usual nonzero-vector definition. Likewise any vector in the nullspace of $C$ is stationary with zero output second moment and need not have the normalized length. These exceptional equilibria must be distinguished from a nonzero feature-learning solution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
