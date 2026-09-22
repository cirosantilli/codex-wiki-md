<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [characteristic polynomial](../../../characteristic-polynomial.md) is

$$
\det(A-\lambda I)=(1-\lambda)(-1-\lambda)+2=\lambda^2+1.
$$

Thus the [eigenvalues](../../../eigenvalue.md) are $i$ and $-i$. There is no real [diagonalization](../../../diagonalization-of-a-matrix.md), because a real [diagonal matrix](../../../diagonal-matrix.md) would have real [eigenvalues](../../../eigenvalue.md). Over the [complex numbers](../../../complex-number.md), the two distinct [eigenvalues](../../../eigenvalue.md) give [linearly independent](../../../linear-independence.md) [eigenvectors](../../../eigenvector.md), so the [matrix](../../../matrix.md) is diagonalizable.

For $\lambda=i$, the first row gives $(1-i)x+2y=0$. Choose $x=2$, giving $y=-1+i$. Its standard complex [norm](../../../norm.md) is $\sqrt{|2|^2+|-1+i|^2}=\sqrt6$; the conjugate [eigenvector](../../../eigenvector.md) belongs to $-i$. Hence normalized [eigenvectors](../../../eigenvector.md) and a suitable [change of basis](../../../change-of-basis.md) are

$$
\boxed{\mathbf p_+=\frac1{\sqrt6}\begin{pmatrix}2\\-1+i\end{pmatrix},\qquad
\mathbf p_-=\frac1{\sqrt6}\begin{pmatrix}2\\-1-i\end{pmatrix},\qquad
P=\frac1{\sqrt6}\begin{pmatrix}2&2\\-1+i&-1-i\end{pmatrix}.}
$$

Directly, $AP=P\operatorname{diag}(i,-i)$ and $\det P=-2i/3\ne0$, so

$$
\boxed{P^{-1}AP=\begin{pmatrix}i&0\\0&-i\end{pmatrix}.}
$$

Normalization does not assert that these [eigenvectors](../../../eigenvector.md) are [orthogonal](../../../orthogonal-vectors.md).

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
