<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the full $3\times3$ [matrix](../../../../../matrix.md) $B$ in the original PDF; the transcription has dropped its middle column. For either [matrix](../../../../../matrix.md), the three-dimensional [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\chi_M(t)=t^3-(\operatorname{tr}M)t^2+[(\operatorname{tr}M)^2-\operatorname{tr}(M^2)]t/2-\det M$. Both have zero [trace](../../../../../matrix-trace.md) and zero [determinant](../../../../../determinant.md), while $\operatorname{tr}(B^2)=0$ and $\operatorname{tr}(C^2)=72$. Consequently

$$
\boxed{\chi_B(t)=t^3,\qquad\chi_C(t)=t(t-6)(t+6).}
$$

For $B$, a useful check is

$$
B^2=\begin{pmatrix}12&0&-24\\18&0&-36\\6&0&-12\end{pmatrix},\qquad B^3=0,
$$

for every value of $\alpha$. Thus $B$ is a nonzero [nilpotent matrix](../../../../../nilpotent-matrix.md) for all $\alpha$; for example its second column never vanishes. By the preceding result, $\boxed{B\text{ is not diagonalizable for any }\alpha}$.

For $C$, the three [eigenvalues](../../../../../eigenvalue.md) $-6,0,6$ are distinct and real, so their [eigenvectors](../../../../../eigenvector.md) are linearly independent. An explicit eigenbasis is

$$
v_- =\begin{pmatrix}-1\\0\\1\end{pmatrix},\qquad v_0=\begin{pmatrix}2\\-3\\1\end{pmatrix},\qquad v_+=\begin{pmatrix}2\\3\\1\end{pmatrix}.
$$

With $P=(v_-,v_0,v_+)$, $\det P=18\neq0$ and $P^{-1}CP=\operatorname{diag}(-6,0,6)$. Hence $\boxed{C\text{ is diagonalizable over }\mathbb R\text{ and }\mathbb C}$.

A repeated root of the [characteristic polynomial](../../../../../characteristic-polynomial.md) alone would not settle diagonalizability; for $B$ it is the nonzero nilpotence that completes the argument.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
