<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Take a code alphabet of size $D\geq2$ and prescribed positive [integer](../../../../../integer.md) lengths $\ell_1,\ldots,\ell_q$. A [decipherable code](../../../../../decipherable-code.md) means that concatenation of codewords determines the entire finite sequence of codewords uniquely. First prove the necessary [Kraft inequality](../../../../../kraft-mcmillan-inequality.md). If $A(m,L)$ counts sequences of $m$ codewords with total length $L$, [unique decodability](../../../../../unique-decodability.md) gives $A(m,L)\leq D^L$. Therefore

$$
K^m:=\left(\sum_{i=1}^qD^{-\ell_i}\right)^m
=\sum_{L=m\ell_{\min}}^{m\ell_{\max}}A(m,L)D^{-L}
\leq m(\ell_{\max}-\ell_{\min})+1.
$$

Taking $m$th roots and letting $m\to\infty$ gives $K\leq1$.

Conversely, order the lengths increasingly and construct a [prefix code](../../../../../prefix-code.md) in the rooted $D$-ary [tree](../../../../../tree-graph-theory.md). At depth $\ell_j$, previously selected codewords forbid exactly $\sum_{i<j}D^{\ell_j-\ell_i}$ vertices. The partial [Kraft inequality](../../../../../kraft-mcmillan-inequality.md) implies

$$
\sum_{i<j}D^{\ell_j-\ell_i}\leq D^{\ell_j}-1,
$$

so an available vertex exists. Select it as the next codeword. Earlier lengths are no greater, so this preserves the [prefix code](../../../../../prefix-code.md) property. A [prefix code](../../../../../prefix-code.md) has [unique decodability](../../../../../unique-decodability.md): in two purported parsings, the first unequal codewords would force one to be a prefix of the other. This proves the [equivalence of decipherable and prefix code lengths](../../../../../equivalence-of-decipherable-and-prefix-code-lengths.md): **the two existence conditions are equivalent**.

For a one-symbol alphabet, at most one positive-length codeword can be decipherable: two different unary codewords commute under concatenation. At most one is also exactly the prefix-code condition, so the equivalence still holds. The same argument covers countably many prescribed positive lengths for $D\geq2$: necessity applies to each finite subset, and $K\leq1$ ensures finitely many words at each length, allowing the ordered construction. Empty codewords are excluded, as required for [unique decodability](../../../../../unique-decodability.md) of arbitrary sequences.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
