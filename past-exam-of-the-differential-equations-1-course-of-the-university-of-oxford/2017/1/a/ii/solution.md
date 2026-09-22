<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $X,Y$ are continuously differentiable near the equilibrium. Put $\xi=x-a$, $\eta=y-b$ and expand the [vector field](../../../../../vector-field.md):

$$
\frac d{dt}\begin{pmatrix}\xi\\\eta\end{pmatrix}=M\begin{pmatrix}\xi\\\eta\end{pmatrix}+o\!\left(\sqrt{\xi^2+\eta^2}\right),\qquad
\boxed{M=\begin{pmatrix}X_x(a,b)&X_y(a,b)\\Y_x(a,b)&Y_y(a,b)\end{pmatrix}.}
$$

This [Jacobian matrix](../../../../../jacobian-matrix.md) defines the linearized system. For distinct real [eigenvalues](../../../../../eigenvalue.md), two negative values give a stable node, two positive values an unstable node, and opposite signs a [saddle point of a dynamical system](../../../../../saddle-equilibrium.md). A complex-conjugate pair with negative real part gives a stable focus, and one with positive real part an unstable focus. Thus a hyperbolic saddle has **two real [eigenvalues](../../../../../eigenvalue.md) of opposite signs**, equivalently $\det M<0$.

The [linearization stability theorem](../../../../../linearization-stability-theorem.md) transfers these stability conclusions to the nonlinear system when no [eigenvalue](../../../../../eigenvalue.md) has zero real part. Distinctness alone is insufficient: a zero eigenvalue or a purely imaginary conjugate pair leaves a [nonhyperbolic equilibrium](../../../../../nonhyperbolic-equilibrium.md), for which the nonlinear terms must be examined. In the purely imaginary case the linearized trajectories form a centre, but that does not establish a nonlinear centre.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
