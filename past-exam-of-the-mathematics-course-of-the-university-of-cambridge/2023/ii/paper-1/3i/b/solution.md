<h1 id="3i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Huffman coding](../../../../../../huffman-coding.md) merges may be chosen as

$$
0.1+0.1=0.2,\qquad
0.2+0.2=0.4,\qquad
0.2+0.4=0.6,\qquad
0.4+0.6=1.
$$

Resolving the tied weights so that the original $0.4$ symbol is merged only at the final step gives the code

$$
\begin{array}{c|ccccc}
\text{probability}&0.4&0.2&0.2&0.1&0.1\\ \hline
\text{codeword}&0&100&101&110&111.
\end{array}
$$

Its lengths are $(1,3,3,3,3)$ and its expected length is

$$
0.4+3(0.2+0.2+0.1+0.1)=\boxed{2.2}.
$$

The [Huffman coding](../../../../../../huffman-coding.md) theorem proves optimality, so an optimal coding with all but one word of the same length does exist. This is an instance of a [nonunique optimal prefix code](../../../../../../nonunique-optimal-prefix-code.md): a different resolution of the ties also gives the optimal profile $(2,2,2,3,3)$.

An optimal code cannot have five distinct lengths. By the [deepest sibling property of an optimal prefix code](../../../../../../deepest-sibling-property-of-an-optimal-prefix-code.md), at least two maximal-length codewords have the same length. Thus the answers are respectively

$$
\boxed{\text{(i) yes},\qquad\text{(ii) no}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3I](../../3i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
