<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $R=1+r$, $m=\mathbb E\xi_1$ and $c=\operatorname{Cov}(S_1,\xi_1)=\mathbb E[(S_1-\mu)(\xi_1-m)]$. The riskless gross return must be nonzero for the requested formulas; in the usual positive-bank-account model $R>0$. If $R=0$, the bank holding cannot affect the terminal payoff, and the later moment equation for pricing $B_0=1$ is impossible. We use the intended nondegenerate case $R\ne0$.

The claim and asset prices are square integrable. Centering separates the bias from the stochastic error:

$$
\mathbb E[(\xi_1-\phi R-\pi\cdot S_1)^2]
=(m-\phi R-\pi\cdot\mu)^2
+\operatorname{Var}(\xi_1)-2\pi^Tc+\pi^TV\pi.
$$

For fixed $\pi$, the unique minimizing bank holding removes the bias. The invertible [covariance matrix](../../../../../../covariance-matrix.md) $V$ is positive definite, and completing the square gives

$$
\pi^TV\pi-2\pi^Tc
=(\pi-V^{-1}c)^TV(\pi-V^{-1}c)-c^TV^{-1}c.
$$

Consequently the unique [one-period quadratic hedge](../../../../../../one-period-quadratic-hedge.md) is

$$
\boxed{\pi^*=V^{-1}c,\qquad \phi^*=\frac{m-(\pi^*)^T\mu}{R}.}
$$

Its minimum expected squared error is $\operatorname{Var}(\xi_1)-c^TV^{-1}c$. This is a least-squares hedge, not necessarily exact [claim replication](../../../../../../claim-replication.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
