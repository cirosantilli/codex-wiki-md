<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

Use [completing the square](../../../../../completing-the-square.md) in the [Hermitian form](../../../../../hermitian-form.md) $x^*Ax$, rather than [unitary diagonalization of a normal matrix](../../../../../unitary-diagonalization-of-a-normal-matrix.md). The first pivot is one, so

$$
x^*Ax=|x_1+ix_2+2ix_3|^2+2|x_2|^2+(-2-i)\overline{x_2}x_3+(-2+i)\overline{x_3}x_2+|x_3|^2.
$$

A second square completion gives

$$
x^*Ax=|x_1+ix_2+2ix_3|^2+2\left|x_2+\frac{-2-i}{2}x_3\right|^2-\frac32|x_3|^2.
$$

Therefore one answer is

$$
\boxed{D=\operatorname{diag}(1,2,-3/2),\qquad T=\begin{pmatrix}1&i&2i\\0&1&(-2-i)/2\\0&0&1\end{pmatrix}.}
$$

The diagonal entries of $D$ are rational, $\det T=1$, and the displayed identity for every $x$ proves $T^*DT=A$.

If $T$ were a [unitary matrix](../../../../../unitary-matrix.md), this [matrix congruence](../../../../../matrix-congruence.md) would also be a [similarity transformation](../../../../../similarity-transformation.md), so the diagonal entries of $D$ would be the [eigenvalues](../../../../../eigenvalue.md) of $A$. Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\det(tI-A)=t^3-9t^2+17t+3=(t-3)(t^2-6t-1).
$$

Thus its [eigenvalues](../../../../../eigenvalue.md) are $3,3+\sqrt{10},3-\sqrt{10}$, two of which are irrational. **A unitary factor cannot give a rational diagonal here.** Alternatively, the permitted [rational root theorem](../../../../../rational-root-theorem.md) implies that three rational eigenvalues would all be integers, whereas the quadratic factor has no integer roots.

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
