<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Put $\varepsilon_n=\sup_{[-1,1]}|F_n-F|$. [Uniform convergence](../../../../../uniform-convergence.md) means $\varepsilon_n\to0$, and continuity ensures that the functions have [Riemann integrals](../../../../../riemann-integral.md). The [integral triangle inequality](../../../../../integral-triangle-inequality.md) gives

$$
\left|\int_{-1}^1F_n(x)\,dx-\int_{-1}^1F(x)\,dx\right|
\leq\int_{-1}^1|F_n(x)-F(x)|\,dx\leq2\varepsilon_n\longrightarrow0.
$$

This proves that [uniform convergence preserves integrals on a compact interval](../../../../../uniform-convergence-preserves-integrals-on-a-compact-interval.md).

For the [derivative](../../../../../derivative.md) assertion, take $F_n(x)=\sin(n^2x)/n$ and $F(x)=0$. These functions are differentiable, with $\sup|F_n|\leq1/n$, so their convergence is uniform. However, **$F_n'(0)=n$ whereas $F'(0)=0$**. The [derivatives](../../../../../derivative.md) therefore need not converge even at one interior point.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
