<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A square [matrix](../../../../matrix.md) is invertible precisely when its [determinant](../../../../determinant.md) is nonzero. Equivalent conditions are full [rank](../../../../rank-one-quadratic-form.md), a trivial [kernel](../../../../kernel-of-a-linear-map-split.md), and zero not being an [eigenvalue](../../../../eigenvalue.md).

For a lower [triangular matrix](../../../../triangular-matrix.md), the first row has only the possibly nonzero entry $A_{11}$. A [Laplace expansion](../../../../laplace-expansion.md) along that row gives $\det A=A_{11}\det A^{(1)}$, where the remaining principal submatrix is again lower triangular. Induction from the one-by-one case yields

$$
\boxed{\det A=\prod_{j=1}^nA_{jj}.}
$$

This proof includes singular triangular matrices; it makes no division by diagonal entries.

For the diagonal example, put $N=n(n+1)/2$. Its [determinant](../../../../determinant.md) is $b^{1+2+\cdots+n}=b^N$, and invertibility requires $b\ne0$. Write the [complex number](../../../../complex-number.md) as $b=re^{i\theta}$ with $r>0$. A nonzero purely imaginary determinant requires $\cos(N\theta)=0$. Thus

$$
\boxed{b=r\exp\left[\frac{(2m+1)\pi i}{n(n+1)}\right],\qquad r>0,\quad m\in\mathbb Z.}
$$

Equivalently $b^N\in i\mathbb R\setminus\{0\}$; the angle is understood modulo $2\pi$.

For [skew-Hermitian matrices](../../../../skew-hermitian-matrix.md), reversing products under the [conjugate transpose](../../../../conjugate-transpose.md) gives $(CD)^\dagger=D^\dagger C^\dagger=DC$. Consequently

$$
\boxed{CD\text{ is skew-Hermitian}\ \Longleftrightarrow\ DC=-CD\ \Longleftrightarrow\ CD+DC=0.}
$$

The latter condition is vanishing of the [anticommutator](../../../../anticommutator.md). A universal choice for the last request is

$$
\boxed{\alpha=-1,\qquad CD-DC=[C,D].}
$$

Indeed $(CD-DC)^\dagger=DC-CD=-(CD-DC)$, so the [commutator](../../../../commutator.md) of two skew-Hermitian matrices is skew-Hermitian.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
