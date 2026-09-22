<h1 id="1d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**True.** All three [eigenvalues](../../../../../../eigenvalue.md) are distinct in $\mathbb C$, so their nonzero [eigenvectors](../../../../../../eigenvector.md) are [linearly independent](../../../../../../linear-independence.md). Here is a direct proof of that assertion. If $a_1v_1+a_2v_2+a_3v_3=0$, apply $(A-\lambda_2I)(A-\lambda_3I)$ to obtain

$$
a_1(\lambda_1-\lambda_2)(\lambda_1-\lambda_3)v_1=0.
$$

Distinctness makes both scalar factors nonzero, hence $a_1=0$. Applying the analogous products gives $a_2=a_3=0$. The three [eigenvectors](../../../../../../eigenvector.md) therefore form a [basis](../../../../../../basis.md) of $\mathbb C^3$. Taking them as the columns of $P$ gives

$$
\boxed{P^{-1}AP=\operatorname{diag}\left(-1,\frac{1+i}{\sqrt2},\frac{1-i}{\sqrt2}\right)}.
$$

This proves that every such matrix is a [diagonalizable matrix](../../../../../../diagonalizable-matrix.md) over $\mathbb C$, rather than merely showing it for the example.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1D](../../1d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
