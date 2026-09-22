<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $m\ge2$, as required for the lower bound in this part. A binary [Huffman code](../../../../../../huffman-code.md) has a [full binary tree](../../../../../../full-binary-tree.md): every merge has two children, and all [codewords](../../../../../../codeword.md) are leaves. More generally an optimal [prefix code](../../../../../../prefix-code.md) for positive-probability symbols cannot have an internal vertex with only one child, since suppressing that vertex shortens its descendant [codewords](../../../../../../codeword.md) and reduces the expected length.

Choose a leaf of maximum depth $s$. Its sibling must also be a leaf, since an internal sibling would have a descendant deeper than $s$. These two leaves give the [deepest sibling property of an optimal prefix code](../../../../../../deepest-sibling-property-of-an-optimal-prefix-code.md), and there are only $m$ leaves altogether. Therefore

$$
\boxed{2\le n_s\le m.}
$$

For the degenerate singleton alphabet, an empty [codeword](../../../../../../codeword.md) suffices and $n_s=1$; the stated lower bound consequently excludes $m=1$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
