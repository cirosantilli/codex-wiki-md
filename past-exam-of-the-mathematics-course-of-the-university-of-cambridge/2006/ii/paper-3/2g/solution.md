<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Introduce $p_{-1}=1$, $q_{-1}=0$, $p_0=a_0$ and $q_0=1$. Composition of the [Möbius transformations](../../../../../mobius-transformation.md) $z\mapsto a_j+1/z$ represents a finite [continued fraction](../../../../../continued-fraction.md). Their [matrices](../../../../../matrix.md) give

$$
\boxed{\begin{pmatrix}p_n&p_{n-1}\\q_n&q_{n-1}\end{pmatrix}=\begin{pmatrix}a_0&1\\1&0\end{pmatrix}\begin{pmatrix}a_1&1\\1&0\end{pmatrix}\cdots\begin{pmatrix}a_n&1\\1&0\end{pmatrix}.}
$$

Indeed, multiplying the last factor gives the [linear recurrences](../../../../../linear-recurrence-relation.md) $p_n=a_np_{n-1}+p_{n-2}$ and $q_n=a_nq_{n-1}+q_{n-2}$, which reproduce the [continued fraction convergents](../../../../../continued-fraction-convergent.md) of the [continued fraction](../../../../../continued-fraction.md). Each factor has [determinant](../../../../../determinant.md) $-1$. Taking [determinants](../../../../../determinant.md) therefore yields

$$
\boxed{p_nq_{n-1}-q_np_{n-1}=(-1)^{n+1}.}
$$

This identity also proves that the numerator and denominator in the first column are [coprime](../../../../../coprime-integers.md), so no unnoticed cancellation changes the displayed [matrix](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
