<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the [covariance matrix](../../../../../../covariance-matrix.md) $\Sigma$ is positive definite and the excess-mean vector $d=z-R\mathbf1$ is nonzero. Put $A=d^t\Sigma^{-1}d>0$. Substituting $w=\lambda\Sigma^{-1}d$ in the mean constraint gives $\lambda A=\mu-R$. Therefore

$$
\boxed{\lambda=\frac{\mu-R}{d^t\Sigma^{-1}d}.}
$$

These weights are indeed the minimum-variance solution, not just a stationary point. Any other feasible vector is $w+v$ with $d^tv=0$. Its [variance](../../../../../../variance-split.md) is $w^t\Sigma w+2\lambda d^tv+v^t\Sigma v=w^t\Sigma w+v^t\Sigma v$, which is strictly larger unless $v=0$. If $d=0$, only mean $R$ is feasible, and the minimum-risk [portfolio](../../../../../../investment-portfolio.md) invests entirely in the [risk-free asset](../../../../../../risk-free-asset.md); the multiplier formula with zero denominator is not applicable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
