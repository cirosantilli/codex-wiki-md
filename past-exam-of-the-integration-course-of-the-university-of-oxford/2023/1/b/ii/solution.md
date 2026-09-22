<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The exact criterion is

$$
\boxed{m(E)<\infty.}
$$

Necessity follows already from one approximation with error less than one: a [compact set](../../../../../compact-space.md) $K\subseteq\mathbb R$ is bounded, hence has finite [Lebesgue measure](../../../../../lebesgue-measure.md), so $m(E)=m(K)+m(E\setminus K)<\infty$.

Conversely, suppose $m(E)<\infty$. By [continuity from above of a measure](../../../../../continuity-from-above-of-a-measure.md), the decreasing sets $E\setminus[-N,N]$ have measures tending to zero. Choose $N\geq1$ so that $m(E\setminus[-N,N])<\varepsilon/2$. Put $B=[-N,N]\setminus E$. By part (b)(i), there is an [open set](../../../../../open-set.md) $V\supseteq B$ with $m(V\setminus B)<\varepsilon/2$. Define

$$
K=[-N,N]\setminus V.
$$

It is closed and bounded, hence a [compact set](../../../../../compact-space.md) by the [Heine-Borel theorem](../../../../../heine-borel-theorem.md), and $K\subseteq E$. The discarded portion satisfies

$$
m(E\setminus K)\leq m(E\setminus[-N,N])+m(E\cap[-N,N]\cap V)<\varepsilon.
$$

The second term is at most $m(V\setminus B)$. This proves the claimed [inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md) with an arbitrarily small absolute error.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
