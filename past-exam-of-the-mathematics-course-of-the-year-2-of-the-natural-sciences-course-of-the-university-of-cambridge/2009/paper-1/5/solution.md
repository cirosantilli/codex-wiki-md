<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [spectral theorem for real symmetric matrices](../../../../spectral-theorem-for-real-symmetric-matrices.md) supplies an [orthonormal basis](../../../../orthonormal-basis.md) of real [eigenvectors](../../../../eigenvector.md). Put these in the columns of $Q$, so $Q^TQ=I$ and $Q^TAQ=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$. In the question's coordinate convention choose $O=Q^T$ and $y=Ox$. Since $x=O^Ty$,

$$
x^TAx=y^TOAO^Ty=\sum_{i=1}^n\lambda_i y_i^2.
$$

Reorder the [eigenvalues](../../../../eigenvalue.md) with $m$ positive, $\ell-m$ negative and $n-\ell$ zero. For nonzero eigenvalues set $z_i=\sqrt{|\lambda_i|}y_i$, and retain the remaining coordinates as $z_i=y_i$. This is an invertible real transformation $z=DOx$, where $D$ is the diagonal rescaling; the combined matrix $L=DO$ gives $z=Lx$. It gives

$$
x^TAx=\sum_{i=1}^mz_i^2-\sum_{i=m+1}^{\ell}z_i^2,
$$

with the zero coordinates absent. The general allowed range is **$0\leq m\leq\ell\leq n$**. The printed restriction $m\geq1$ is not valid for every real symmetric matrix: a negative-definite or zero form has no positive square. The invariance of these counts is [Sylvester's law of inertia](../../../../sylvester-s-law-of-inertia.md).

For the specified form, a particularly simple change is

$$
\boxed{z=Lx,\quad L=\begin{pmatrix}1/2&1/2&1/2\\1/2&-1/2&-1/2\\0&1&-1\end{pmatrix},\qquad x_1x_2+x_1x_3=z_1^2-z_2^2.}
$$

Subtracting the first two squared coordinates verifies the identity directly, and $\det L=1$ proves invertibility. Thus $m=1$, $\ell=2$ and there is one zero direction. The final rescaling need not remain orthogonal.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
