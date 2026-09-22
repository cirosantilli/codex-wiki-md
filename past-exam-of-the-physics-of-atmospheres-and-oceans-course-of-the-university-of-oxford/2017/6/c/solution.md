<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [instantaneous Lorenz error growth at a zero-y crossing](../../../../instantaneous-lorenz-error-growth-at-a-zero-y-crossing.md), direct differentiation of the [Lorenz system](../../../../lorenz-system.md) gives

$$
J=\begin{pmatrix}-\sigma&\sigma&0\\r-z&-1&-x\\y&x&-b\end{pmatrix}.
$$

At a crossing of $y=0$ its [symmetric part](../../../../symmetric-matrix.md) is particularly simple:

$$
\boxed{S=J+J^T=\begin{pmatrix}-2\sigma&\sigma+r-z&0\\
\sigma+r-z&-2&0\\0&0&-2b\end{pmatrix}.}
$$

Thus a perturbation initially in the $z$ direction has norm-squared rate $-2b$ and initially decays in [norm](../../../../norm.md) at rate $b$. The $x$-dependent couplings between $y$ and $z$ are [skew-symmetric](../../../../skew-symmetric-matrix.md) at the crossing and do not contribute to the instantaneous total [norm](../../../../norm.md) derivative. They can rotate the perturbation later: a pure $\delta z$ immediately induces $\dot{\delta y}=-x\delta z$. It is therefore incorrect to claim that such an error remains an independently decaying $z$ mode along the complete trajectory.

For the $(x,y)$ block, the [trace](../../../../matrix-trace.md) is $-2(\sigma+1)<0$ and the [determinant](../../../../determinant.md) is $4\sigma-(\sigma+r-z)^2$. A negative [determinant](../../../../determinant.md) gives one positive and one negative [eigenvalue](../../../../eigenvalue.md). Equivalently,

$$
\lambda_\pm=-(\sigma+1)\pm\sqrt{(\sigma-1)^2+(\sigma+r-z)^2},
\qquad \lambda_+>0\iff|\sigma+r-z|>2\sqrt\sigma.
$$

In particular the requested sufficient lower-height condition is

$$
\boxed{z<F(\sigma,r),\qquad F(\sigma,r)=\sigma+r-2\sqrt\sigma.}
$$

There is also a second growth range $z>\sigma+r+2\sqrt\sigma$; it must not be lost by removing the absolute value. At either endpoint the largest rate is zero. Between them both block [eigenvalues](../../../../eigenvalue.md) are negative. At a crossing in either growing range, some planar error directions have positive instantaneous exponential rate. This statement is local in time: a single instantaneous positive [eigenvalue](../../../../eigenvalue.md) of $S$ does not prove sustained exponential error growth over an evolving Lorenz trajectory.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
