<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [seasonal difference operator](../../../../../../seasonal-difference-operator.md) has $b_0=1$, $b_{12}=-1$ and all other coefficients zero. Its frequency response is $1-e^{12i\lambda}$, so

$$
\boxed{f_Z(\lambda)=4\sin^2(6\lambda)f_Y(\lambda),\qquad
G_b(\lambda)=2|\sin(6\lambda)|.}
$$

The right sketch shows zeros at $\lambda=j\pi/6$ for $j=0,\ldots,6$, and maxima of height two at $(2j+1)\pi/12$ for $j=0,\ldots,5$. The [seasonal difference operator](../../../../../../seasonal-difference-operator.md) removes every exactly twelve-periodic component, including a constant. Its [filter gain](../../../../../../filter-gain.md) has a comb pattern: it selectively suppresses seasonal frequencies, rather than increasing monotonically with frequency.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
