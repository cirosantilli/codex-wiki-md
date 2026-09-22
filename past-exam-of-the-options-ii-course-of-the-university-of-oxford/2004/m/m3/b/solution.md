<h1 id="m/m3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The independent identically distributed [central limit theorem](../../../../../central-limit-theorem.md) states that for variables of common finite mean $\mu$ and finite positive [variance](../../../../../variance-split.md) $\sigma^2$,

$$
\frac{\sum_{i=1}^nX_i-n\mu}{\sigma\sqrt n}\ \xrightarrow{d}\ N(0,1).
$$

For the [exponential distribution](../../../../../exponential-distribution.md), $\mu=1/\lambda$ and $\sigma=1/\lambda$. Thus the event in question is exactly

$$
\left\{\frac{\lambda\sum_{i=1}^nX_i-n}{\sqrt n}<x\right\}.
$$

The limiting [normal distribution](../../../../../normal-distribution.md) has a continuous distribution function at every real $x$, so [convergence in distribution](../../../../../convergence-in-distribution.md) gives

$$
\boxed{\mathbb P\left(\sum_{i=1}^nX_i<\frac{n+x\sqrt n}{\lambda}\right)\longrightarrow\Phi(x)}.
$$

Here $\Phi(x)=(2\pi)^{-1/2}\int_{-\infty}^xe^{-u^2/2}\,du$, including the strict-inequality convention because the limiting distribution is continuous.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M3](../../m3.md)
3. [M](../../../m.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
