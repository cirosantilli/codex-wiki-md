<h1 id="8b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Partial fractions give $f(z)=-1/(z-1)+1/(z-2)$. In the interior [disk](../../../../../../disk-mathematics.md), expand both terms as [geometric series](../../../../../../geometric-series.md):

$$
-\frac1{z-1}=\sum_{n=0}^\infty z^n,\qquad
\frac1{z-2}=-\sum_{n=0}^\infty\frac{z^n}{2^{n+1}}.
$$

Thus the [Laurent series](../../../../../../laurent-series.md) is a [Taylor series](../../../../../../taylor-series.md) in this region:

$$
\boxed{f(z)=\sum_{n=0}^\infty(1-2^{-n-1})z^n},\qquad |z|<1.
$$

The nearer [pole](../../../../../../pole.md) at $z=1$ determines the radius of convergence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8B](../../8b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
