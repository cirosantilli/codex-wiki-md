<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

By [Jordan normal form](../../../../jordan-normal-form.md), each complex [nilpotent matrix](../../../../nilpotent-matrix.md) of size six can be put by [matrix similarity](../../../../matrix-similarity.md) into a [block diagonal matrix](../../../../block-diagonal-matrix.md) whose [Nilpotent Jordan blocks](../../../../nilpotent-jordan-block.md) have sizes

$$
s_1\geq s_2\geq\cdots\geq s_k\geq1,\qquad \sum_{j=1}^k s_j=6.
$$

A [Nilpotent Jordan block](../../../../nilpotent-jordan-block.md) of size $s$ has [matrix rank](../../../../matrix-rank.md) $s-1$ and [minimal polynomial](../../../../minimal-polynomial.md) $t^s$. Therefore, for the whole [matrix](../../../../matrix.md),

$$
\operatorname{rank}A=\sum_{j=1}^k(s_j-1)=6-k,\qquad m_A(t)=t^{s_1}.
$$

Thus the given [matrix rank](../../../../matrix-rank.md) determines the number $k$ of [Jordan blocks](../../../../jordan-block.md), and the given [minimal polynomial](../../../../minimal-polynomial.md) determines the largest size $s_1$. For size six these two data determine the entire [integer partition](../../../../integer-partition.md). Here is the complete list, arranged by the largest size:

$$
\begin{array}{c|c|c}
\text{block sizes}&k&\operatorname{rank}A\\\hline
(6)&1&5\\
(5,1)&2&4\\
(4,2)&2&4\\
(4,1,1)&3&3\\
(3,3)&2&4\\
(3,2,1)&3&3\\
(3,1,1,1)&4&2\\
(2,2,2)&3&3\\
(2,2,1,1)&4&2\\
(2,1,1,1,1)&5&1\\
(1,1,1,1,1,1)&6&0
\end{array}
$$

To see that the list is exhaustive, choose the largest part $s_1$ between one and six and partition the remainder $6-s_1$ into parts at most $s_1$. The resulting rows all have distinct pairs $(s_1,k)$. Hence $A$ and $B$ have the same [Jordan normal form](../../../../jordan-normal-form.md) $J$.

Explicitly, choose [invertible matrices](../../../../invertible-matrix.md) $X,Y$ such that $A=XJX^{-1}$ and $B=YJY^{-1}$. Then

$$
\boxed{P=XY^{-1}\quad\Longrightarrow\quad P^{-1}AP=YJY^{-1}=B.}
$$

This proves [matrix similarity](../../../../matrix-similarity.md) and illustrates the [classification of six-dimensional nilpotent matrices by rank and nilpotency index](../../../../classification-of-six-dimensional-nilpotent-matrices-by-rank-and-nilpotency-index.md).

## ↑ Ancestors (12)

1. [b](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
