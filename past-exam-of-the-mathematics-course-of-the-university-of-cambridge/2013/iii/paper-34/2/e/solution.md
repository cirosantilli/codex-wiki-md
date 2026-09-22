<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The normalized [log-uniform distribution](../../../../../../log-uniform-distribution.md) here has density $1/(x\log10)$. A leading digit $i$ corresponds to $i\le X<i+1$, so

$$
\boxed{\mathbb P(D=i)=\frac1{\log10}\int_i^{i+1}\frac{dx}{x}
=\log_{10}(1+1/i),\qquad i=1,\ldots,9.}
$$

These are exactly the [Benford law](../../../../../../benford-law.md) probabilities. Continuous densities make endpoint conventions immaterial.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
