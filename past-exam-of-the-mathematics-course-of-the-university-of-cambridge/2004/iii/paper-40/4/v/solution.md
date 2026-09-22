<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Take $k>0$, so the proposal is the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,k]$, with [probability density function](../../../../../../probability-density-function.md) $g(x)=1/k$. Symmetry of the standard [Cauchy distribution](../../../../../../cauchy-distribution.md) gives

$$
\mu=\frac12-\int_0^kf(x)\,dx
=\frac12-k\mathbb E_g[f(X)].
$$

Thus the proposed expression is exactly the unbiased [importance sampling](../../../../../../importance-sampling.md) estimator of this complementary [integral](../../../../../../integral.md):

$$
\boxed{\widehat\mu=\frac12-\frac{k}{n}\sum_{i=1}^n\frac1{\pi(1+x_i^2)}.}
$$

It has finite [variance](../../../../../../variance-split.md) because $f$ is bounded on $[0,k]$. Explicitly,

$$
\begin{aligned}
\mathbb E_gf(X)&=\frac{\arctan k}{\pi k},\\
\mathbb E_gf(X)^2&=\frac1{2\pi^2k}\left(\arctan k+\frac{k}{1+k^2}\right),\\
\operatorname{Var}(\widehat\mu)
&=\frac1{n\pi^2}\left[\frac{k}{2}\left(\arctan k+\frac{k}{1+k^2}\right)-(\arctan k)^2\right].
\end{aligned}
$$

These follow from the antiderivatives of $(1+x^2)^{-1}$ and $(1+x^2)^{-2}$. The target itself is $\mu=1/2-\arctan(k)/\pi$. At $k=0$ it is exactly $1/2$ without simulation; for negative $k$ the printed uniform-interval construction must be changed.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
