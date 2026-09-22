<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [union bound](../../../../../../../boole-s-inequality.md),

$$
\mathbb P_p(0\leftrightarrow\partial B(n))
\leq\sum_{z\in\partial B(n)}
\mathbb P_p(0\leftrightarrow z).
$$

Hence some $z\in\partial B(n)$ has connection probability at least the left side divided by $|\partial B(n)|$. Some coordinate of $z$ equals $n$ or $-n$. A coordinate permutation and reflection of $\mathbb Z^d$ sends that face to the face $x_1=n$ and preserves the [bond percolation](../../../../../../../bond-percolation-split.md) law. Its image $x$ therefore satisfies

$$
\boxed{\mathbb P_p(0\leftrightarrow x)
\geq\frac{\mathbb P_p(0\leftrightarrow\partial B(n))}{|\partial B(n)|}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
