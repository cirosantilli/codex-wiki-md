<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For times $t_1,\ldots,t_n<1$ and real coefficients $a_i$, the [linear combination](../../../../../../linear-combination.md) of coordinates is

$$
\sum_i a_iX_{t_i}=\int_0^{\max_i t_i}\left(\sum_i\frac{a_i(1-t_i)\mathbf1_{[0,t_i]}(s)}{1-s}\right)dB_s.
$$

The [Gaussianity of deterministic Brownian stochastic integrals](../../../../../../gaussianity-of-deterministic-brownian-stochastic-integrals.md) makes this a centered [normal random variable](../../../../../../gaussian-random-variable.md). Indeed step-function approximations give [linear combinations](../../../../../../linear-combination.md) of independent normal increments, and the [Itô isometry](../../../../../../ito-isometry.md) gives convergence in $L^2$; their [characteristic functions](../../../../../../characteristic-function.md) converge to that of a normal variable with the limiting variance. Since every [linear combination](../../../../../../linear-combination.md) is normal, the coordinate vector is a [Gaussian random vector](../../../../../../gaussian-random-vector.md). Appending the deterministic coordinate $X_1=0$ preserves that property, so $X$ is a centered [Gaussian process](../../../../../../gaussian-process.md) on $[0,1]$.

For $0\le s\le t<1$, the [covariance](../../../../../../covariance.md) version of the [Itô isometry](../../../../../../ito-isometry.md) gives

$$
\mathbb E[X_sX_t]=(1-s)(1-t)\int_0^s\frac{du}{(1-u)^2}
=(1-s)(1-t)\frac{s}{1-s}=s(1-t).
$$

At $t=1$ the [covariance](../../../../../../covariance.md) is zero because $X_1=0$, agreeing with the formula. Thus the [Brownian bridge covariance kernel](../../../../../../brownian-bridge-covariance-kernel.md) is

$$
\boxed{\Gamma(s,t)=\min(s,t)-st,\qquad\mathbb EX_t=0}.
$$

Its finite-dimensional distributions identify it as a [Brownian bridge](../../../../../../brownian-bridge.md); continuity at the terminal endpoint is established next.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
