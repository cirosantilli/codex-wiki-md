<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Let $n=2^l-1$ and let $H$ be the $l\times n$ [parity-check matrix](../../../../../parity-check-matrix.md) whose columns are the distinct nonzero vectors of the [finite field](../../../../../finite-field.md) vector space $\mathbb F_2^l$. The binary [Hamming code](../../../../../hamming-code.md) is

$$
C=\ker H=\{x\in\mathbb F_2^n:Hx^T=0\}.
$$

A [perfect code](../../../../../perfect-code.md) has [Hamming balls](../../../../../hamming-ball.md) of radius $t=\lfloor(d-1)/2\rfloor$ about its codewords partitioning the whole ambient space, where $d$ is its [minimum Hamming distance of a linear code](../../../../../minimum-hamming-distance-of-a-linear-code.md).

No column of $H$ is zero and no two columns agree, so $C$ has no word of [Hamming weight](../../../../../hamming-weight.md) one or two. Three suitable columns sum to zero, so $d=3$. For any received word $y$, its [syndrome](../../../../../syndrome.md) $Hy^T$ is either zero or is the unique column $h_i$ of $H$ equal to that syndrome. In the first case $y\in C$; in the second,

$$
H(y+e_i)^T=Hy^T+h_i=0,
$$

so $y$ is at [Hamming distance](../../../../../hamming-distance.md) one from a codeword. Uniqueness follows from $d=3$. Thus the radius-one balls partition $\mathbb F_2^n$, and the code is perfect.

For $l=3$, the [dual code](../../../../../dual-code.md) is the [binary simplex code](../../../../../binary-simplex-code.md) of length seven. Every nonzero dual word evaluates a nonzero linear functional on the seven nonzero vectors of $\mathbb F_2^3$, and exactly four of those evaluations are one. Hence every nonzero word of $C^\perp$ has weight

$$
\boxed{4}.
$$

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
