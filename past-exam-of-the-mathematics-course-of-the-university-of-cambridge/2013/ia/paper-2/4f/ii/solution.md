<h1 id="4f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Poisson distribution](../../../../../../poisson-distribution.md) with unit parameter has mass $e^{-1}/j!$. Its [moment-generating function](../../../../../../moment-generating-function.md) is

$$
\boxed{\mathbb E[e^{tX}]=e^{-1}\sum_{j=0}^\infty\frac{e^{tj}}{j!}
=\exp(e^t-1)}.
$$

For an integer $k\geq1$, multiply the exponential [probability](../../../../../../probability.md) bound by $e$ to obtain $\sum_{j=k}^\infty1/j!\leq\exp(e^t-kt)$. The exponent is minimized at $e^t=k$, hence $t=\log k\geq0$, including $t=0$ when $k=1$. Consequently

$$
\boxed{\sum_{j=k}^\infty\frac1{j!}\leq e^{k-k\log k}=\left(\frac ek\right)^k}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
