<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

With $q=2\lambda+1$, the reduced coefficient matrix and its symmetric part are

$$
A=\begin{pmatrix}-q^2/2&2\alpha\\-2\alpha&-(q^2+1)/2\end{pmatrix},
\qquad
A_s=\frac{A+A^T}{2}
=-\frac12\begin{pmatrix}q^2&0\\0&q^2+1\end{pmatrix}.
$$

Its diagonal entries are both strictly negative exactly when $q\ne0$, equivalently $\boxed{\lambda\ne-1/2}$. The coherent driving cancels from the symmetric part because it is a rotation generator.

For a [steady state](../../../../../../steady-state.md) $s_*$ put $e=s-s_*$. Differentiating the squared Euclidean distance gives

$$
\frac d{dt}\|e\|^2=e^T(A+A^T)e
=-q^2e_x^2-(q^2+1)e_z^2
\leq-q^2\|e\|^2.
$$

For $q\ne0$ the derivative is strictly negative whenever $e\ne0$. Integrating the inequality proves the [symmetric-part contraction criterion](../../../../../../symmetric-part-contraction-criterion.md) here explicitly:

$$
\boxed{\|s(t)-s_*\|\leq e^{-q^2t/2}\|s(0)-s_*\|.}
$$

Thus every nonstationary initial state approaches the unique [steady state](../../../../../../steady-state.md), with strictly decreasing distance; the [steady state](../../../../../../steady-state.md) itself has constant zero distance. If the decoupled $y$ coordinate is retained, it contributes $-e_y^2$ to the squared-distance derivative and also decays, so the conclusion holds for the full qubit state.

For the target-dependent settings in (e), $q=-\cos\theta_d$. Every nonequatorial target is therefore globally attractive. At an equatorial target, $q=\alpha=0$: $x(t)=x(0)$, $z(t)=z(0)e^{-t/2}$, and $y(t)=y(0)e^{-t/2}$. A general state approaches $(x(0),0,0)$ rather than the specified pure target $x=\pm1$. This proves the equatorial exception, not merely failure of a sufficient estimate.

The parameter dependence matters: $q=0$ alone does not exclude attractivity for every possible driving strength. If $\alpha\ne0$, the reduced matrix has negative [trace](../../../../../../matrix-trace.md) and positive [determinant](../../../../../../determinant.md) $4\alpha^2$, so both [eigenvalues](../../../../../../eigenvalue.md) have negative real parts even though its symmetric part is only semidefinite. The nonattractive case asserted for the equatorial target also uses its prescribed $\alpha=0$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
