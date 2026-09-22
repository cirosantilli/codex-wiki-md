<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [quadratic form](../../../../../quadratic-form-split.md) is $\mathbf x^TQ\mathbf x$ for the real [symmetric matrix](../../../../../symmetric-matrix.md)

$$
Q=\begin{pmatrix}5&0&3\\0&-3&0\\3&0&-3\end{pmatrix}.
$$

The $y$ axis has [eigenvalue](../../../../../eigenvalue.md) $-3$. On the $xz$ plane, the [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\det\begin{pmatrix}5-\ell&3\\3&-3-\ell\end{pmatrix}=(5-\ell)(-3-\ell)-9=\ell^2-2\ell-24=(\ell-6)(\ell+4).
$$

Thus the [orthogonal diagonalization](../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) from part (a) yields

$$
\boxed{\lambda=6,\qquad\mu=-3,\qquad\nu=-4,\qquad6u^2-3v^2-4w^2=\alpha.}
$$

For later use, one possible [orthonormal basis](../../../../../orthonormal-basis.md) is

$$
e_u=\frac{(3,0,1)}{\sqrt{10}},\qquad e_v=(0,1,0),\qquad e_w=\frac{(1,0,-3)}{\sqrt{10}}.
$$

Then $u=(3x+z)/\sqrt{10}$, $v=y$, $w=(x-3z)/\sqrt{10}$. This explicit choice also confirms that the [Euclidean norm](../../../../../euclidean-norm.md) is preserved: $x^2+y^2+z^2=u^2+v^2+w^2$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
