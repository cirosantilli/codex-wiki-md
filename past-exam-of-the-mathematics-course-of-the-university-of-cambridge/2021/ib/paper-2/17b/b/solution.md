<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Starting with $A_1=A$, for $k=1,\ldots,n-2$ choose a [Householder reflection](../../../../../../householder-transformation.md) $H_k$ that acts only on coordinates $k+1,\ldots,n$ and maps the tail of column $k$,

$$
(A_k)_{k+1:n,k},
$$

to a multiple of its first coordinate vector. Set

$$
A_{k+1}=H_kA_kH_k.
$$

This zeros all entries in column $k$ below its first subdiagonal. Because $H_k$ fixes the first $k$ coordinates, it preserves the zeros created in earlier columns. After $n-2$ steps,

$$
T=A_{n-1}
$$

is an [upper Hessenberg matrix](../../../../../../upper-hessenberg-matrix.md).

Each $H_k$ is [orthogonal](../../../../../../orthogonal-matrix.md) and symmetric. If

$$
Q=H_{n-2}\cdots H_1,
$$

then $Q$ is orthogonal and

$$
\boxed{T=QAQ^T}.
$$

Part (a) shows that each similarity update costs $O(n^2)$ arithmetic operations, and there are $O(n)$ updates. The total cost is therefore

$$
\boxed{O(n^3)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
