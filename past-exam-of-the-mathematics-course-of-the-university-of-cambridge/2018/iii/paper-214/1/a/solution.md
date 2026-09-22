<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [bond percolation](../../../../../../bond-percolation-split.md), the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) states that any two [increasing events](../../../../../../increasing-event.md) $A,B$ satisfy

$$
\mathbb P_p(A\cap B)\geq\mathbb P_p(A)\mathbb P_p(B).
$$

The same inequality holds for two [decreasing events](../../../../../../decreasing-event.md), either by reversing the coordinate order or by taking complements in the two-event identity. Intersections of [decreasing events](../../../../../../decreasing-event.md) are [decreasing events](../../../../../../decreasing-event.md), so induction gives

$$
\mathbb P_p\left(\bigcap_{j=1}^n A_j^c\right)\geq\prod_{j=1}^n\mathbb P_p(A_j^c).
$$

Write $a=\mathbb P_p(A_1)=\cdots=\mathbb P_p(A_n)$ and $u=\mathbb P_p(\bigcup_jA_j)$. Then $1-u\geq(1-a)^n$. Taking the nonnegative $n$-th root and rearranging yields the [square-root trick for positively associated events](../../../../../../square-root-trick-for-positively-associated-events.md):

$$
\boxed{\mathbb P_p(A_1)\geq1-\left(1-\mathbb P_p\left(\bigcup_{j=1}^n A_j\right)\right)^{1/n}.}
$$

No independence among the events is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
