<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The interior grid is $x=1,2,3$, with fixed-end [displacements](../../../../../displacement.md) $u_0=u_4=0$. Hence

$$
\boxed{A=\begin{pmatrix}-2&1&0\\1&-2&1\\0&1&-2\end{pmatrix}.}
$$

Use the monic [characteristic polynomial](../../../../../characteristic-polynomial.md) convention $p(\lambda)=\det(\lambda I-A)$, where $I$ is the [identity matrix](../../../../../identity-matrix.md). Expansion of the [determinant](../../../../../determinant.md) along the first row gives

$$
\begin{aligned}
p(\lambda)
&=\det\begin{pmatrix}\lambda+2&-1&0\\-1&\lambda+2&-1\\0&-1&\lambda+2\end{pmatrix}\\
&=(\lambda+2)\bigl((\lambda+2)^2-1\bigr)-(\lambda+2)\\
&=\boxed{(\lambda+2)\bigl((\lambda+2)^2-2\bigr)
=\lambda^3+6\lambda^2+10\lambda+4.}
\end{aligned}
$$

The [eigenvalues](../../../../../eigenvalue.md) are the [roots of a polynomial](../../../../../root-of-a-polynomial.md) $p(\lambda)=0$. With the alternative [determinant](../../../../../determinant.md) convention $\det(A-\lambda I)$, the [characteristic polynomial](../../../../../characteristic-polynomial.md) is $-p(\lambda)$ because the [matrix](../../../../../matrix.md) has odd size; its [roots of a polynomial](../../../../../root-of-a-polynomial.md) are unchanged.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
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
