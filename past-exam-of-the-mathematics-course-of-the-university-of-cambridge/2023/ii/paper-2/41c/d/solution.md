<h1 id="41c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Using [Euler's formula](../../../../../../euler-s-formula.md),

$$
\cos(\pi x)=\frac12e^{i\pi x}+\frac12e^{-i\pi x},
$$



$$
-\frac12\sin(\pi x)
=\frac i4e^{i\pi x}-\frac i4e^{-i\pi x}.
$$

Thus

$$
\widehat c_0=2,
\qquad
\widehat c_1=\frac12+\frac i4,
\qquad
\widehat c_{-1}=\frac12-\frac i4.
$$

Ordering the modes as $(-1,0,1)$, let $a=1/2+i/4$. Then

$$
C=\begin{pmatrix}
2&\overline a&0\\
a&2&\overline a\\
0&a&2
\end{pmatrix},
\qquad
D=\begin{pmatrix}-1&0&0\\0&0&0\\0&0&1\end{pmatrix}.
$$

Consequently

$$
\boxed{
B=-CD=
\begin{pmatrix}
2&0&0\\
\frac12+\frac i4&0&-\frac12+\frac i4\\
0&0&-2
\end{pmatrix}.}
$$

This matrix is [triangular](../../../../../../triangular-matrix.md), so its eigenvalues are its diagonal entries:

$$
\boxed{\operatorname{spec}(B)=\{-2,0,2\}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [41C](../../41c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
