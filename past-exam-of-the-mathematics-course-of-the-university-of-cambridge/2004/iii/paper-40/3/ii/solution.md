<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For rate $\lambda>0$, return

$$
\boxed{X=-\frac1\lambda\log U_1.}
$$

For $x\geq0$, $\mathbb P(X>x)=\mathbb P(U_1<e^{-\lambda x})=e^{-\lambda x}$, so $X$ has the [exponential distribution](../../../../../../exponential-distribution.md) of rate $\lambda$. This is [inverse transform sampling](../../../../../../inverse-transform-sampling.md); using $-\log(1-U_1)/\lambda$ is equivalent. Uniform draws at exact endpoints can be excluded, since those events have [probability](../../../../../../probability.md) zero under the ideal continuous law.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
