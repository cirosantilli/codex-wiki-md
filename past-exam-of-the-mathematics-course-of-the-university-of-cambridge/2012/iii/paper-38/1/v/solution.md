<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For the causal case $|\phi|<1$, expand

$$
\frac{1+\theta B}{1-\phi B}
=1+\sum_{j\ge1}(\phi+\theta)\phi^{j-1}B^j.
$$

Hence the [white noise](../../../../../../white-noise.md) coefficients are $\psi_0=1$ and $\psi_j=(\phi+\theta)\phi^{j-1}$ for $j\ge1$. Orthogonality of [white noise](../../../../../../white-noise.md) gives $\gamma_k=\sigma^2\sum_{j\ge0}\psi_j\psi_{j+k}$ for $k\ge0$. Summing the [geometric series](../../../../../../geometric-series.md) yields the [autocovariance of a causal ARMA(1,1) process](../../../../../../autocovariance-of-a-causal-arma-1-1-process.md):

$$
\boxed{\gamma_0=\frac{\sigma^2(1+\theta^2+2\phi\theta)}{1-\phi^2},
\qquad
\gamma_k=\frac{\sigma^2(\phi+\theta)(1+\phi\theta)}{1-\phi^2}
\phi^{k-1}\quad(k\ge1),\qquad\gamma_{-k}=\gamma_k.}
$$

For $\phi=0$, this means $\gamma_1=\sigma^2\theta$ and $\gamma_k=0$ for $k\ge2$, together with $\gamma_0=\sigma^2(1+\theta^2)$. For $\theta=-\phi$, all positive-lag [covariances](../../../../../../covariance.md) vanish and $\gamma_0=\sigma^2$, as expected from cancellation of the two filter polynomials.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
