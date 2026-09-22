<h1 id="6b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $q=e^{-\lambda t}$ and propose $P_n=q(1-q)^{n-1}$. The initial condition follows from $q(0)=1$. Since $q'=-\lambda q$,

$$
\frac{dP_n}{dt}
=-\lambda q(1-q)^{n-1}
+\lambda(n-1)q^2(1-q)^{n-2}.
$$

On the other hand,

$$
\lambda(n-1)P_{n-1}-\lambda nP_n
=\lambda(n-1)q(1-q)^{n-2}-\lambda nq(1-q)^{n-1},
$$

and expanding the bracket gives the same expression. The formula also sums to one by the [geometric series](../../../../../../geometric-series.md), so it is the required [probability mass function](../../../../../../probability-mass-function.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
