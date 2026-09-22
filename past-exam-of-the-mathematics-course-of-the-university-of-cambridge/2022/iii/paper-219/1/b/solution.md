<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [Cepheid](../../../../../../cepheid-variable.md) measurement as $\widehat\mu=\mu+\epsilon_\mu$, where $\epsilon_\mu\sim N(0,\sigma_\mu^2)$, and define the calibrated [absolute magnitude](../../../../../../absolute-magnitude.md) data

$$
q_k=m_k-\widehat\mu
=M_0+\Delta M_G+\delta M_k-\epsilon_\mu.
$$

Thus $q=(q_1,\ldots,q_K)^T$ has a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) with mean $M_0\mathbf1$ and [covariance matrix](../../../../../../covariance-matrix.md)

$$
C=\sigma_I^2I_K+(\sigma_G^2+\sigma_\mu^2)\mathbf1\mathbf1^T.
$$

The [Hubble law](../../../../../../hubble-s-law.md) and the definition of [distance modulus](../../../../../../distance-modulus.md) give

$$
m_i=M_i+25+5\log_{10}\!\left(\frac{cz_i}{100\ {\rm km\,s}^{-1}}\right)-\theta.
$$

Consequently, with

$$
x_i=m_i-25-5\log_{10}\!\left(\frac{cz_i}{100\ {\rm km\,s}^{-1}}\right),
$$

the Hubble-flow observations are [independent random variables](../../../../../../independent-random-variables.md) satisfying $x_i\sim N(M_0-\theta,\sigma_{\rm tot}^2)$. Apart from a factor independent of the parameters, the joint [likelihood function](../../../../../../likelihood-function.md) is

$$
L(M_0,\theta)
\propto |C|^{-1/2}
\exp\!\left[-\frac12(q-M_0\mathbf1)^TC^{-1}(q-M_0\mathbf1)\right]
(\sigma_{\rm tot}^2)^{-N/2}
\exp\!\left[-\frac1{2\sigma_{\rm tot}^2}
\sum_{i=1}^N\{x_i-(M_0-\theta)\}^2\right].
$$

The expression extends by continuity to a singular limiting covariance such as $\sigma_I=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
