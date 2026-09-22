<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [diagonalization](../../../../../diagonalization-of-a-matrix.md) in part (b) gives $M^k=P\operatorname{diag}(a^k,b^k,c^k)P^{-1}$. Hence

$$
\boxed{M^k\to0\ \Longleftrightarrow\ |a|<1,\ |b|<1,\ |c|<1.}
$$

Sufficiency follows from the scalar powers tending to zero; necessity also follows immediately from the diagonal entries of $M^k$. Under these conditions the [matrix geometric series](../../../../../matrix-geometric-series.md) converges, and its sum is

$$
(I-M)^{-1}=P\operatorname{diag}\left(\frac1{1-a},\frac1{1-b},\frac1{1-c}\right)P^{-1}.
$$

Writing $A_0=1/(1-a)$, $B_0=1/(1-b)$ and $C_0=1/(1-c)$, all entries are explicitly

$$
\boxed{(I-M)^{-1}=\begin{pmatrix}A_0&B_0-A_0&C_0-B_0\\0&B_0&C_0-B_0\\0&0&C_0\end{pmatrix}.}
$$

For example, $B_0-A_0=(b-a)/[(1-a)(1-b)]$ and $C_0-B_0=(c-b)/[(1-b)(1-c)]$. These expressions remain valid when parameter values coincide.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
