<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $W_n$ be the interpolation in part (a). The operation

$$
I:C[0,1]\longrightarrow\mathbb R,\qquad I(f)=\int_0^1f(t)\,dt
$$

is continuous, since $|I(f)-I(g)|\leq\|f-g\|_\infty$. By the [Donsker invariance principle](../../../../../../donsker-s-theorem.md) and the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md),

$$
I(W_n)\xrightarrow{\ d\ }\int_0^1B_t\,dt.
$$

The exact trapezoidal integral of the linear interpolation is

$$
I(W_n)=\frac1{n^{3/2}}
\left(\sum_{k=1}^{n-1}S_k+\frac12S_n\right).
$$

Therefore the statistic in question differs from $I(W_n)$ by $S_n/(2n^{3/2})$. Using [independence](../../../../../../independent-random-variables.md), zero means, and unit variances gives

$$
\mathbb E\left[\left(\frac{S_n}{2n^{3/2}}\right)^2\right]
=\frac{n}{4n^3}=\frac1{4n^2}\longrightarrow0.
$$

This error tends to zero in $L^2$, hence in probability. The [Slutsky theorem](../../../../../../slutsky-theorem.md) now proves the [integrated random-walk limit](../../../../../../integrated-random-walk-limit.md):

$$
\boxed{\frac1{n^{3/2}}\sum_{k=1}^nS_k
\xrightarrow{\ d\ }\int_0^1B_t\,dt.}
$$

The limiting law can also be made explicit. The time integral is a Gaussian [random variable](../../../../../../random-variable-split.md), as a mean-square limit of linear combinations of a [Gaussian process](../../../../../../gaussian-process.md). It is centered, and the [covariance](../../../../../../covariance.md) identity $\mathbb E(B_sB_t)=\min(s,t)$ gives

$$
\operatorname{Var}\left(\int_0^1B_t\,dt\right)
=\int_0^1\int_0^1\min(s,t)\,ds\,dt
=2\int_0^1\int_0^t s\,ds\,dt=\frac13.
$$

Thus the terminal value of [integrated Brownian motion](../../../../../../integrated-brownian-motion.md) here has law **$N(0,1/3)$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
