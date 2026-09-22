<h1 id="3k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [binary block code](../../../../../../binary-block-code.md), $n$ is the common length of its codewords, $m=|C|$ is the number of codewords, and

$$
d=\min_{\substack{x,y\in C\\x\ne y}}d_H(x,y)
$$

is its minimum [Hamming distance](../../../../../../hamming-distance.md).

The [parity extension](../../../../../../parity-extension.md) is

$$
C^+=\left\{
\left(x_1,\ldots,x_n,\sum_{j=1}^nx_j\right):x\in C
\right\}.
$$

Every extended word has even [Hamming weight](../../../../../../hamming-weight.md). The distance between two words increases by one exactly when their original distance is odd, so

$$
\boxed{
C^+\text{ has parameters }[n+1,m,d^+],
\qquad
d^+=
\begin{cases}
d,&d\text{ even},\\
d+1,&d\text{ odd}.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3K](../../3k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
