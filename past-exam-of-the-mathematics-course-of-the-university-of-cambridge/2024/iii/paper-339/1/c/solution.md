<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\lambda^*$ be an optimal dual multiplier and define the maximum violation

$$
v(x)=\max\{0,(Ax-b)_1,\ldots,(Ax-b)_m\}.
$$

Dual stationarity and [strong duality](../../../../../../strong-duality.md) imply, for every $x$,

$$
c^Tx+(\lambda^*)^T(Ax-b)
=-b^T\lambda^*=p^*.
$$

Since every component of $Ax-b$ is at most $v(x)$ and $\lambda^*\geq0$,

$$
(\lambda^*)^T(Ax-b)\leq
\lVert\lambda^*\rVert_1v(x).
$$

It follows that the [exact maximum-violation penalty](../../../../../../exact-maximum-violation-penalty.md) obeys

$$
c^Tx+Mv(x)
\geq p^*+\bigl(M-\lVert\lambda^*\rVert_1\bigr)v(x).
$$

Choose any $M>\lVert\lambda^*\rVert_1$. A primal optimum has $v(x)=0$ and penalized value $p^*$, whereas every infeasible point has $v(x)>0$ and penalized value strictly greater than $p^*$. Thus the penalized problem and the original [linear program](../../../../../../linear-programming.md) have exactly the same minimizers.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
