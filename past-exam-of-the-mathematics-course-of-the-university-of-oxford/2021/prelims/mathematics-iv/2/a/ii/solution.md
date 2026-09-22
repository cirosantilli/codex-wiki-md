<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Represent the [quadratic form](../../../../../../../quadratic-form-split.md) by the [symmetric matrix](../../../../../../../symmetric-matrix.md)

$$
M=\begin{pmatrix}\alpha&\beta/2\\\beta/2&\gamma\end{pmatrix},\qquad
\mathbf x^TM\mathbf x=1.
$$

The [spectral theorem for real symmetric matrices](../../../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives an [orthogonal matrix](../../../../../../../orthogonal-matrix.md) $Q$ and real [eigenvalues](../../../../../../../eigenvalue.md) $\lambda_1,\lambda_2$ such that $Q^TMQ=\operatorname{diag}(\lambda_1,\lambda_2)$. In the [orthogonal change of coordinates](../../../../../../../orthogonal-change-of-coordinates.md) $\mathbf x=Q\mathbf u$, the [equation](../../../../../../../equation.md) becomes $\lambda_1u_1^2+\lambda_2u_2^2=1$.

If both [eigenvalues](../../../../../../../eigenvalue.md) are positive, this is an [ellipse](../../../../../../../ellipse.md) with semiaxes $\lambda_1^{-1/2}$ and $\lambda_2^{-1/2}$. Conversely, a zero [eigenvalue](../../../../../../../eigenvalue.md) makes the set either empty or unbounded along that [coordinate](../../../../../../../coordinate-linear-algebra.md), while two negative [eigenvalues](../../../../../../../eigenvalue.md) give the empty set. Opposite signs give an unbounded [hyperbola](../../../../../../../hyperbola.md). A negative [eigenvalue](../../../../../../../eigenvalue.md) together with a zero one also gives the empty set. None of those cases is an [ellipse](../../../../../../../ellipse.md). Therefore the exact condition is that $M$ be a [symmetric positive-definite matrix](../../../../../../../symmetric-positive-definite-matrix.md).

The sum and product of its [eigenvalues](../../../../../../../eigenvalue.md) are its [matrix trace](../../../../../../../matrix-trace.md) and [determinant](../../../../../../../determinant.md):

$$
\lambda_1+\lambda_2=\alpha+\gamma,\qquad
\lambda_1\lambda_2=\alpha\gamma-\frac{\beta^2}{4}.
$$

Two real numbers are both positive precisely when their sum and product are positive. Thus

$$
\boxed{\alpha+\gamma>0,\qquad 4\alpha\gamma>\beta^2.}
$$

An [orthogonal transformation](../../../../../../../orthogonal-transformation.md) preserves [area](../../../../../../../surface-area.md). Using [i](../i.md) gives the [quadratic-form ellipse area](../../../../../../../quadratic-form-ellipse-area.md)

$$
\boxed{\mathcal A=\frac{\pi}{\sqrt{\det M}}=\frac{2\pi}{\sqrt{4\alpha\gamma-\beta^2}}.}
$$

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [2](../../../2.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
