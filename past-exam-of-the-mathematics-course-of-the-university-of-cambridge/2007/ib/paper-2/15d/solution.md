<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

The [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) satisfies the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md)

$$
y_0L(y;\lambda_0)-yL(y_0;\lambda_0)
=\frac{d}{dx}\bigl[p(y_0y'-yy_0')\bigr].
$$

Indeed the potential terms cancel, and differentiating the right side gives the remaining two derivative terms. Integrate over $[0,1]$. The common [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) make the endpoint term zero, while $L(y_0;\lambda_0)=0$. Therefore

$$
\boxed{\int_0^1y_0f\,dx=0.}
$$

This is the necessary [solvability condition](../../../../../solvability-condition.md) imposed by the nonzero homogeneous solution; its proof here does not rely on merely quoting the [Fredholm alternative](../../../../../fredholm-alternative.md).

For the nonlinear problem, choose

$$
f=L(y;\lambda_0)=y^3-(\lambda-\lambda_0)wy
=y^3-\epsilon^2\mu wy.
$$

The orthogonality condition then gives

$$
\epsilon^2\mu\int_0^1wy_0y\,dx=\int_0^1y_0y^3\,dx.
$$

With $y=\epsilon y_0+\epsilon^2y_1$, where the correction remains bounded as $\epsilon\to0$, the normalization gives

$$
\int_0^1wy_0y\,dx=\epsilon+O(\epsilon^2),\qquad
\int_0^1y_0y^3\,dx=\epsilon^3\int_0^1y_0^4\,dx+O(\epsilon^4).
$$

Divide by $\epsilon^3$ and use $\mu=O(1)$ to obtain

$$
\boxed{\mu=\int_0^1y_0^4\,dx+O(\epsilon).}
$$

The positive quartic integral determines the leading direction of the nonlinear shift from the linear [eigenvalue](../../../../../eigenvalue.md).

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
