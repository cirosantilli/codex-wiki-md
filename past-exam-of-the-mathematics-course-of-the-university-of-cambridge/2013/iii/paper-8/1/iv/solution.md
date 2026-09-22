<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [absolute Fourier convergence from a square-integrable derivative](../../../../../../absolute-fourier-convergence-from-a-square-integrable-derivative.md) uses more than the pointwise estimate $|\widehat f(n)|=O(1/|n|)$. Periodic [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\widehat{f'}(n)=in\widehat f(n).
$$

By [Bessel's inequality](../../../../../../bessel-s-inequality.md),

$$
\sum_{n\ne0}n^2|\widehat f(n)|^2
=\sum_{n\ne0}|\widehat{f'}(n)|^2
\leq\|f'\|_2^2.
$$

Now apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md):

$$
\boxed{\sum_{n\ne0}|\widehat f(n)|
\leq\left(\sum_{n\ne0}n^2|\widehat f(n)|^2\right)^{1/2}
\left(\sum_{n\ne0}\frac1{n^2}\right)^{1/2}
\leq\frac{\pi}{\sqrt3}\|f'\|_2.}
$$

Adding the finite constant coefficient proves absolute summability. Since a continuously differentiable periodic function has $f'\in L^2$, all hypotheses of part (iii) hold and its [Fourier series](../../../../../../fourier-series-split.md) converges uniformly.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
