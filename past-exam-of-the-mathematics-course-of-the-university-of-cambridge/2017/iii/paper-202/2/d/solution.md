<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For continuous [semimartingales](../../../../../../semimartingale.md), the [Stratonovich integral](../../../../../../stratonovich-integral.md) adds half the [quadratic covariation](../../../../../../quadratic-covariation.md) to the [Itô integral](../../../../../../ito-integral.md):

$$
\boxed{S_t=I_t+\frac12[X,Y]_t.}
$$

One can see the factor directly from symmetric endpoint sums. On a [partition of an interval](../../../../../../partition-of-an-interval.md), replacing $X$ at the left endpoint by the average of its two endpoint values adds $\frac12\sum\Delta X\Delta Y$; its limit is $\frac12[X,Y]$. Thus the correction depends only on the continuous [local martingale](../../../../../../local-martingale.md) parts of the [semimartingales](../../../../../../semimartingale.md). If either integrator or integrand has [finite variation](../../../../../../total-variation-of-a-function.md), the [quadratic covariation](../../../../../../quadratic-covariation.md) vanishes and these two integrals coincide. Here the printed notation $\partial Y$ denotes [Stratonovich integral](../../../../../../stratonovich-integral.md) integration, equivalently $\circ dY$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
