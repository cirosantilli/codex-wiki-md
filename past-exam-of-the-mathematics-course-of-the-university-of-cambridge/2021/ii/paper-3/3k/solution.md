<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

Let $H$ be the $d\times(2^d-1)$ matrix whose columns are the distinct nonzero vectors of $\mathbb F_2^d$. The [binary Hamming code](../../../../../hamming-code.md) is

$$
C=\ker H.
$$

No column is zero and no two columns agree, so its minimum distance is three. A radius-one Hamming ball contains

$$
1+(2^d-1)=2^d
$$

words, while $|C|=2^{2^d-1-d}$. The radius-one balls about codewords are disjoint and their total size is $2^{2^d-1}$, so they partition the ambient space. Hence $C$ is a [perfect code](../../../../../perfectness-of-a-hamming-code.md).

Let the received word be all ones except in the last coordinate. The sum of all nonzero vectors of $\mathbb F_2^d$ is zero for $d\geq2$, so its syndrome is the last column of $H$. Minimum-distance decoding therefore flips the last bit and returns the all-one word. A Hamming code corrects every single error because each nonzero syndrome identifies its unique erroneous coordinate.

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
