<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

The change of variable $x=(y/\lambda)^k$ has [derivative](../../../../../derivative.md) $kx/y$, so

$$
f_\lambda(y)=e^{-(y/\lambda)^k}\frac{k}{\lambda}\left(\frac y\lambda\right)^{k-1},\qquad y>0.
$$

For fixed $k$ this is

$$
k y^{k-1}\exp\left\{\eta y^k-A(\eta)\right\},\qquad
\eta=-\lambda^{-k}<0,\quad A(\eta)=-\log(-\eta).
$$

Thus the sample's [sufficient statistic](../../../../../sufficient-statistic.md) is $T=\sum_iY_i^k$.

Since $(Y/\lambda)^k\sim\operatorname{Exp}(1)$,

$$
\mathbb E(Y^k)=\lambda^k.
$$

The log likelihood, up to constants, is $-kn\log\lambda-T/\lambda^k$. Differentiating gives the unique maximum

$$
\boxed{\widehat\lambda=\left(\frac1n\sum_{i=1}^nY_i^k\right)^{1/k}.}
$$

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
