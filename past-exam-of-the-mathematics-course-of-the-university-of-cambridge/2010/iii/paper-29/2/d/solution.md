<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) and [Brownian scaling](../../../../../../brownian-scaling.md) give

$$
\mathbb P\left(\sup_{s\le K^2}B_s>r\right)
=2\mathbb P(B_{K^2}>r)=2\mathbb P(Z>r/K),
$$

where $Z$ has the standard [normal distribution](../../../../../../normal-distribution.md). Combine part (c) with the allowed [Gaussian tail bound](../../../../../../gaussian-tail-bound.md) to obtain

$$
\boxed{\mathbb P(|f(X)-\mu|>r)\le4\exp\left(-\frac{r^2}{2K^2}\right).}
$$

This is the [Brownian martingale proof of Gaussian concentration](../../../../../../brownian-martingale-proof-of-gaussian-concentration.md). It proves the intended [Gaussian concentration inequality](../../../../../../gaussian-concentration-inequality.md). The denominator printed in the initial bound is $2K$, whereas the gradient hypothesis and part (c) give $2K^2$. The stronger printed bound is false in general. For a concrete counterexample, take $d=1$, $K=2$, and $f(x)=2x$. At $r=10$,

$$
\mathbb P(|f(Z)|>10)=2\mathbb P(Z>5)
>\frac{2}{\sqrt{2\pi}}e^{-18}>4e^{-25},
$$

where the first strict inequality follows by integrating the decreasing normal density over $[5,6]$. The rightmost term is the printed bound. Thus the square on $K$ is a necessary source correction, rather than a change of proof technique.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
