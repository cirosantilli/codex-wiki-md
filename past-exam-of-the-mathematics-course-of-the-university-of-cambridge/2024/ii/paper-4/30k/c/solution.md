<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [matrix](../../../../../../matrix.md)

$$
P=X^T(XX^T)^{-1}X
$$

is the orthogonal projection onto the row space of $X$. Since $XP\beta=X\beta$, the empirical risks of $h_\beta$ and $h_{P\beta}$ are equal. Orthogonality gives

$$
\|\beta\|^2=\|P\beta\|^2+\|(I-P)\beta\|^2,
$$

so $q(\beta)\geq q(P\beta)$, with strict inequality unless $(I-P)\beta=0$. Therefore the minimizer lies in the row space:

$$
\widehat\beta=P\widehat\beta=X^T\widehat\alpha.
$$

Because $X^T$ is injective when $XX^T$ is invertible, minimizing over that row space is equivalent to minimizing $r(\alpha)=q(X^T\alpha)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
