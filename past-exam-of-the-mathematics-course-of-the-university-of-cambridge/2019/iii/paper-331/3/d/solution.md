<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Differentiate the quadratic [energy](../../../../../../energy.md):

$$
\dot E=2\lambda_1x_1^2+2x_1x_2+2\lambda_2x_2^2=2x^THx,\qquad H=\frac{L+L^T}{2}=\begin{pmatrix}\lambda_1&1/2\\1/2&\lambda_2\end{pmatrix}.
$$

For $x_1\ne0$, put $r=x_2/x_1$. Immediate energy growth occurs precisely when $\lambda_2r^2+r+\lambda_1>0$. With both [eigenvalues](../../../../../../eigenvalue.md) negative, such directions exist iff $1-4\lambda_1\lambda_2>0$. Writing $\delta=\sqrt{1-4\lambda_1\lambda_2}$, the growing initial conditions are the two opposite open wedges

$$
\boxed{x_1\ne0,\qquad \frac{-1+\delta}{2\lambda_2}<\frac{x_2}{x_1}<\frac{-1-\delta}{2\lambda_2}.}
$$

If $x_1=0$, energy decreases. No energy growth at any time, for any initial condition, is possible exactly when

$$
\boxed{\lambda_1\lambda_2\geq\frac14\quad(\lambda_1,\lambda_2<0).}
$$

Indeed, this makes the [symmetric part of a matrix](../../../../../../symmetric-part-of-a-matrix.md) $H$ a [negative semidefinite matrix](../../../../../../negative-semidefinite-matrix.md), so $\dot E\leq0$ along every trajectory. If the product is smaller, the wedges already supply counterexamples at $t=0$. This is the [instantaneous energy-growth criterion for a linear system](../../../../../../instantaneous-energy-growth-criterion-for-a-linear-system.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
