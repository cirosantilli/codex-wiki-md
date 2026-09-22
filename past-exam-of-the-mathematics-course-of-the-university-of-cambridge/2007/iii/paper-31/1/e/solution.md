<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [full binary tree](../../../../../../full-binary-tree.md) has Kraft sum one. For example, place mass one at the root and divide each internal vertex's mass equally between its children; a leaf at depth $l$ receives $2^{-l}$, and the total mass on leaves remains one. Using part d gives the two equations

$$
n_{s-1}+n_s=m,\qquad \frac{n_{s-1}}{2^{s-1}}+\frac{n_s}{2^s}=1.
$$

Multiplying the second equation by $2^s$ and subtracting the first gives the [uniform-source Huffman length distribution](../../../../../../uniform-source-huffman-length-distribution.md)

$$
\boxed{n_{s-1}=2^s-m,\qquad n_s=2m-2^s,\qquad s=\lceil\log_2m\rceil.}
$$

If $m=2^s$, the first number is zero and every [codeword](../../../../../../codeword.md) has length $s$. Otherwise both levels occur. The corresponding mean length is $L=s-(2^s-m)/m$.

## ↑ Ancestors (11)

1. [E](../e.md)
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
