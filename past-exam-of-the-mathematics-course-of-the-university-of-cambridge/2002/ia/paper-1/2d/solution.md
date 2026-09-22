<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

The [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) says that every nonconstant [polynomial](../../../../../polynomial-split.md) with [complex number](../../../../../complex-number.md) coefficients has a root in the [complex numbers](../../../../../complex-number.md). Repeated [polynomial division](../../../../../polynomial-division.md) by a factor of degree one therefore factors a degree-three [polynomial](../../../../../polynomial-split.md) with [complex number](../../../../../complex-number.md) coefficients into three factors of degree one, with [algebraic multiplicities](../../../../../algebraic-multiplicity.md) included.

For a [matrix](../../../../../matrix.md) with [complex number](../../../../../complex-number.md) entries $A$ of size three, its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\chi_A(t)=\det(tI-A)$, and its characteristic equation is $\chi_A(t)=0$. A [complex number](../../../../../complex-number.md) $\lambda$ is an [eigenvalue](../../../../../eigenvalue.md) exactly when $\lambda I-A$ is singular, equivalently when its [null space](../../../../../kernel-of-a-linear-map.md) contains a nonzero [vector](../../../../../vector.md). Thus the three roots of the [characteristic polynomial](../../../../../characteristic-polynomial.md) are the three [eigenvalues](../../../../../eigenvalue.md) counted with [algebraic multiplicity](../../../../../algebraic-multiplicity.md).

For the specified [matrix](../../../../../matrix.md), expansion along the first row gives

$$
\chi_A(t)=(t-1)\det\begin{pmatrix}t&-i\\i&t\end{pmatrix}
=(t-1)(t^2-1)=(t-1)^2(t+1).
$$

Hence **the [eigenvalues](../../../../../eigenvalue.md) are $1,1,-1$**. Corresponding [eigenvectors](../../../../../eigenvector.md) are

$$
v_1=\begin{pmatrix}1\\0\\0\end{pmatrix},\qquad
v_2=\begin{pmatrix}0\\i\\1\end{pmatrix},\qquad
v_3=\begin{pmatrix}0\\-i\\1\end{pmatrix},
\qquad Av_1=v_1,\quad Av_2=v_2,\quad Av_3=-v_3.
$$

The [matrix](../../../../../matrix.md) with these three columns has [determinant](../../../../../determinant.md) $2i\ne0$, so these [eigenvectors](../../../../../eigenvector.md) are [linearly independent](../../../../../linear-independence.md). A repeated [eigenvalue](../../../../../eigenvalue.md) does not in general guarantee two independent [eigenvectors](../../../../../eigenvector.md); here they have been exhibited directly.

## ↑ Ancestors (11)

1. [2D](../2d.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
