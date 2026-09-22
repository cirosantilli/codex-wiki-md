<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Keep $y$ fixed. Integral bounds for the decreasing function $1/t$ give $H_M=\log M+O(1)$, so $H_M-H_{y-1}=\log M+O_y(1)$. Consequently

$$
\boxed{\mathbb E[N\mid y,M]\frac{\log M}{M}
=\frac{M-y+1}{M}\frac{\log M}{H_M-H_{y-1}}\longrightarrow1.}
$$

The [posterior mean](../../../../../../posterior-mean.md) thus grows like $M/\log M$ instead of approaching a data-determined limit. Even the [posterior distribution](../../../../../../bayesian-posterior.md) mass below a fixed endpoint $n$ is $(H_n-H_{y-1})/(H_M-H_{y-1})\to0$. Hence increasing the supposedly innocuous prior cutoff moves the inference to larger and larger endpoints. In an integral approximation its median is of order $\sqrt{yM}$, also depending strongly on the cutoff. This explains the sensitivity of the entire inference, not just of its [posterior mean](../../../../../../posterior-mean.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
