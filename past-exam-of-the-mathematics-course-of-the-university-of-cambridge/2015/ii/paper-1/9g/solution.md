<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

For $r\geq2$, let $H$ be the $r\times(2^r-1)$ binary [matrix](../../../../../matrix.md) whose columns are all distinct nonzero vectors of $\mathbb F_2^r$. The binary [Hamming code](../../../../../hamming-code.md) is $C=\ker H$. Its [parity-check matrix](../../../../../parity-check-matrix.md) has rank $r$ since its columns include the standard basis. Hence $C$ is linear of length $2^r-1$ and dimension $2^r-1-r$.

No word of weight one or two lies in $C$, since columns are nonzero and distinct; three columns $u,v,u+v$ sum to zero, so the [minimum distance of a code](../../../../../minimum-distance-of-a-code.md) is exactly three. The [syndrome](../../../../../syndrome.md) of a single-bit error is its column of $H$, uniquely identifying the erroneous position. The $2^r$ possible syndromes correspond to no error or exactly one of $2^r-1$ single-bit errors. Alternatively, every radius-one [Hamming ball](../../../../../hamming-ball.md) has $2^r$ words and

$$
|C|\,2^r=2^{2^r-1-r}2^r=2^{2^r-1}.
$$

Disjoint balls therefore cover the whole word space. This proves **linearity, one-error correction and perfection**. For $r=3$, the parameters are $[7,4,3]$, giving the 16 messages needed below.

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
