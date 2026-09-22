<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write

$$
C=A_0A_1\cdots A_r.
$$

Under the improved bounds allowed in the question, $r=O(\log^{O(1)}(2K))$ and

$$
|C|\geq\exp\bigl(-O(\log^{O(1)}(2K))\bigr)|A|.
$$

Moreover $AC\subseteq A^{O(1)}$, whose size is at most $K^{O(1)}|A|$ by the [higher product bound for an approximate group](../../../../../../../higher-product-bound-for-an-approximate-group.md). Thus

$$
|AC|\leq\exp\bigl(O(\log^{O(1)}(2K))\bigr)|C|.
$$

The [Ruzsa covering lemma](../../../../../../../ruzsa-covering-lemma.md) supplies $X\subseteq A$ of size at most $\exp(O(\log^{O(1)}(2K)))$ such that

$$
A\subseteq XCC^{-1}
=XA_0A_1\cdots A_rA_r\cdots A_1A_0.
$$

Taking the $B_i$ to be the factors in this last product gives

$$
\boxed{A\subseteq XB_1\cdots B_k,}
$$

where $k\leq O(\log^{O(1)}(2K))$ and every $B_i$ is a $K^{O(1)}$-approximate group in $A^{O(1)}$ generating a subgroup of step less than $s$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 149](../../../../paper-149-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
