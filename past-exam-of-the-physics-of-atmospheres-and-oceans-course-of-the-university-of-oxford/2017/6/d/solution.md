<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At the specified state, the [symmetric matrix](../../../../symmetric-matrix.md) is

$$
S=\begin{pmatrix}-20&12&0\\12&-2&0\\0&0&-6\end{pmatrix}.
$$

The planar characteristic equation is $\lambda^2+22\lambda-104=0$, giving $4$ and $-26$, while the third [eigenvalue](../../../../eigenvalue.md) is $-6$. An orthonormal set of [eigenvectors](../../../../eigenvector.md) is

$$
\boxed{\lambda_1=4,\quad\mathbf e_1=\frac{(1,2,0)^T}{\sqrt5};\qquad
\lambda_2=-26,\quad\mathbf e_2=\frac{(-2,1,0)^T}{\sqrt5};\qquad
\lambda_3=-6,\quad\mathbf e_3=(0,0,1)^T.}
$$

With comparable prior uncertainty in these dimensionless coordinates and equally accurate scalar observations, prioritize the growing combination

$$
\boxed{y_{\rm obs}\propto x+2y.}
$$

An observation of this projection removes error in the direction that grows most strongly over a sufficiently short forecast; its [norm](../../../../norm.md) initially grows at rate $2$ in Lorenz time units. The strongly contracting direction is a lower priority under those assumptions. This is not an observation of the absolute state amplitude alone: the relevant error projection is $(\delta x+2\delta y)/\sqrt5$. Anisotropic [prior covariance](../../../../covariance-matrix.md), observation noise or a different forecast [norm](../../../../norm.md) would modify the optimal choice; for a finite forecast the leading [right singular vector](../../../../right-singular-vector.md) of the actual [propagator](../../../../fundamental-matrix-of-a-linear-differential-equation.md) replaces this instantaneous direction.

## ↑ Ancestors (12)

1. [D](../d.md)
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
