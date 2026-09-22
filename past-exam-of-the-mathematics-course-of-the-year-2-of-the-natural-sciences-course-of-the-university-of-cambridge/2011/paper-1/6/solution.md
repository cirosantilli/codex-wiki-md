<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Over the chosen scalar field, an $n$-by-$n$ [matrix](../../../../matrix.md) is [diagonalizable](../../../../diagonalizable-matrix.md) if and only if it has $n$ [linearly independent](../../../../linear-independence.md) [eigenvectors](../../../../eigenvector.md). Repeated eigenvalues are allowed provided all [eigenspaces](../../../../eigenspace.md) together supply a basis.

For the given matrix, the [characteristic polynomial](../../../../characteristic-polynomial.md) is $\lambda^2-4\lambda-5=(\lambda-5)(\lambda+1)$. One may choose

$$
\boxed{\lambda_1=5,\quad V_1=\begin{pmatrix}5\\1\end{pmatrix},\qquad\lambda_2=-1,\quad V_2=\begin{pmatrix}-1\\1\end{pmatrix}.}
$$

Taking these as columns gives the [change of basis](../../../../change-of-basis.md)

$$
\boxed{P=\begin{pmatrix}5&-1\\1&1\end{pmatrix},\qquad P^{-1}=\frac16\begin{pmatrix}1&1\\-1&5\end{pmatrix},\qquad P^{-1}AP=\begin{pmatrix}5&0\\0&-1\end{pmatrix}.}
$$

**This is not a rotation matrix.** The PDF's terminology cannot hold literally: $A$ is real and nonsymmetric, whereas a real matrix orthogonally similar to a real diagonal matrix is symmetric. Also $V_1\cdot V_2=-4\ne0$, so scaling these eigenvectors cannot make an orthonormal rotation basis. A general invertible similarity is the valid construction.

Let $D=P^{-1}AP$. Inserting $PP^{-1}$ between successive factors gives $A^n=PD^nP^{-1}$, and hence

$$
\boxed{P^{-1}A^nP=\operatorname{diag}(5^n,(-1)^n).}
$$

To write $A^n=\alpha_nA+\beta_nI$, match its action on the two eigenspaces:

$$
5\alpha_n+\beta_n=5^n,\qquad-\alpha_n+\beta_n=(-1)^n.
$$

Solving gives the [matrix powers for a diagonalizable matrix with two eigenvalues](../../../../matrix-powers-for-a-diagonalizable-matrix-with-two-eigenvalues.md)

$$
\boxed{A^n=\frac{5^n+(-1)^{n+1}}6A+\frac{5^n+5(-1)^n}6I,\qquad n\geq0.}
$$

The cases $n=0,1$ recover $I,A$, respectively. Equivalently the [spectral projections of a diagonalizable matrix](../../../../spectral-projection-of-a-diagonalizable-matrix.md) are $(A+I)/6$ and $(5I-A)/6$, and the power multiplies them by $5^n$ and $(-1)^n$.

## ↑ Ancestors (12)

1. [6](../6.md)
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
