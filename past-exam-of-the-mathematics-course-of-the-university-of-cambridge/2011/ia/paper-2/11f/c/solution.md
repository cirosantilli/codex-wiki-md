<h1 id="11f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The homogeneous [linear recurrence relation](../../../../../../linear-recurrence-relation.md) has characteristic polynomial $(\lambda-1)^2$, hence general solution $h_k=A+Bk$. For the expected-time recurrence, rearrangement gives $m_{k+1}-2m_k+m_{k-1}=-2$, for which $-k^2$ is a particular solution. Thus

$$
\boxed{h_k=A+Bk,\qquad m_k=C+Dk-k^2.}
$$

Imposing the absorbing [boundary conditions](../../../../../../boundary-condition.md) from the preceding parts gives the [gambler's ruin](../../../../../../gambler-s-ruin.md) formulas

$$
\boxed{h_k=\frac{k}{20},\qquad m_k=k(20-k).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [11F](../../11f.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
