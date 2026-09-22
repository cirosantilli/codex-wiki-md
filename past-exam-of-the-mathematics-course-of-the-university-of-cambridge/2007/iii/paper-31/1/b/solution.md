<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If all leaves of a [full binary tree](../../../../../../full-binary-tree.md) have depth $s$, all binary paths of length $s$ end in leaves. Thus it has exactly $2^s$ leaves and $m=2^s$. Equivalently, equality in the [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md) gives $m2^{-s}=1$.

Conversely, when $m=2^k$ a complete depth-$k$ tree is a [prefix code](../../../../../../prefix-code.md) with mean length $k$. For any prefix lengths $s_i$, convexity gives

$$
2^{-L}\le\frac1m\sum_{i=1}^m2^{-s_i}\le\frac1m,\qquad L=\frac1m\sum_i s_i,
$$

so $L\ge\log_2m=k$. The complete tree is optimal. A [Huffman code](../../../../../../huffman-code.md) attains this optimum, and equality in the strictly convex first inequality forces all its lengths to equal $k$. Hence, for $m\ge2$,

$$
\boxed{n_s=m\quad\Longleftrightarrow\quad m\text{ is a power of two}.}
$$

This also proves that ties in the Huffman construction do not change the conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
