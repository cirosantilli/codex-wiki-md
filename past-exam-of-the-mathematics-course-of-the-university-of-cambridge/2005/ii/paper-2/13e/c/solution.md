<h1 id="13e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $u=1+\widehat u(t)\cos(s/L)$ and $v=1+\widehat v(t)\cos(s/L)$ and retain linear terms. With $k=1/L$, the [Fourier mode](../../../../../../fourier-mode.md) has second derivative $-k^2\cos(ks)$. Hence

$$
\boxed{\frac d{dt}\begin{pmatrix}\widehat u\\\widehat v\end{pmatrix}
=\begin{pmatrix}1-k^2&-1\\2Q&-Q(1+Pk^2)\end{pmatrix}
\begin{pmatrix}\widehat u\\\widehat v\end{pmatrix}.}
$$

The trace and [determinant](../../../../../../determinant.md) of this [linearization](../../../../../../linearization.md) are

$$
T(k)=1-Q-(1+QP)k^2,
\qquad D(k)=Q[1+(1-P)k^2+Pk^4].
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13E](../../13e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
