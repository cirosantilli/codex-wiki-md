<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Gaussian elimination](../../../../../gaussian-elimination.md) to the supplied nonsymmetric [matrix](../../../../../matrix.md),

$$
A=\begin{pmatrix}-2&1&0&1\\2&-2&0&0\\0&1&-2&1\\0&0&2&-2\end{pmatrix}.
$$

The first [pivot element](../../../../../pivot-element.md) is $-2$, with [elimination multiplier](../../../../../elimination-multiplier.md) $l_{21}=2/(-2)=-1$. Perform $R_2\leftarrow R_2+R_1$, giving

$$
\begin{pmatrix}-2&1&0&1\\0&-1&0&1\\0&1&-2&1\\0&0&2&-2\end{pmatrix}.
$$

The second [pivot element](../../../../../pivot-element.md) is $-1$, with [elimination multiplier](../../../../../elimination-multiplier.md) $l_{32}=-1$. Perform $R_3\leftarrow R_3+R_2$, then use the third [pivot element](../../../../../pivot-element.md) $-2$ and [elimination multiplier](../../../../../elimination-multiplier.md) $l_{43}=-1$ to perform $R_4\leftarrow R_4+R_3$. The [LU factorization](../../../../../lu-decomposition.md) is

$$
\boxed{A=LU,\qquad
L=\begin{pmatrix}1&0&0&0\\-1&1&0&0\\0&-1&1&0\\0&0&-1&1\end{pmatrix},\qquad
U=\begin{pmatrix}-2&1&0&1\\0&-1&0&1\\0&0&-2&2\\0&0&0&0\end{pmatrix}.}
$$

Here $L$ is a unit [lower triangular matrix](../../../../../lower-triangular-matrix.md), hence an [invertible matrix](../../../../../invertible-matrix.md), and $U$ is an [upper triangular matrix](../../../../../upper-triangular-matrix.md). No row interchange is needed: all three [pivot elements](../../../../../pivot-element.md) used in elimination are nonzero. The final diagonal entry is zero, with an entirely zero last row; there is no further division by it. The three nonzero rows of $U$ are [linearly independent](../../../../../linear-independence.md), so **the [matrix rank](../../../../../matrix-rank.md) is $3$** and $A$ is a [singular matrix](../../../../../singular-matrix.md). Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives $LU=A$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
