<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $P=QQ^T$. Since $Q$ has $r$ columns, the [rank bound for a matrix product](../../../../../rank-bound-for-a-matrix-product.md) gives $\operatorname{rank}(PA)\leq r$. The [Eckart-Young-Mirsky theorem](../../../../../eckart-young-mirsky-theorem.md) and part (a) then give

$$
\boxed{\|PA-A\|_2\geq\sigma_{r+1}=\|Q_*Q_*^TA-A\|_2}.
$$

One can also see the lower bound directly. The restriction of $PA$ to the $(r+1)$-dimensional [linear span](../../../../../linear-span.md) of $v_1,\ldots,v_{r+1}$ has a nonzero [null space](../../../../../kernel-of-a-linear-map-split.md), because its [matrix rank](../../../../../matrix-rank.md) is at most $r$. For a [unit vector](../../../../../unit-vector.md) $z$ in that [null space](../../../../../kernel-of-a-linear-map-split.md), $\|(A-PA)z\|_2=\|Az\|_2\geq\sigma_{r+1}$ by the [singular value decomposition](../../../../../singular-value-decomposition.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
