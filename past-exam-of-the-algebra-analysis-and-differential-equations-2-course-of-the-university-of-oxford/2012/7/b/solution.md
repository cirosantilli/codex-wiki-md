<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first component of the [vector field](../../../../vector-field.md) vanishes only when $y=0$ or $x=\pm1$. The second vanishes only when $y=1$ or $x+y=3$. Intersecting these alternatives gives exactly five [equilibria](../../../../equilibrium-point-of-a-dynamical-system.md). Their [Jacobian matrix](../../../../jacobian-matrix.md) is

$$
M(x,y)=\begin{pmatrix}2xy&x^2-1\\y-1&x+2y-4\end{pmatrix}.
$$

At $(3,0)$,

$$
M=\begin{pmatrix}0&8\\-1&-1\end{pmatrix},\qquad\det(\lambda I-M)=\lambda^2+\lambda+8,\qquad\lambda=\frac{-1\pm i\sqrt{31}}2.
$$

The real parts are negative and the imaginary parts are nonzero, so **$(3,0)$ is a [stable spiral](../../../../stable-spiral.md)**.

At $(1,1)$ the [Jacobian matrix](../../../../jacobian-matrix.md) is $\operatorname{diag}(2,-1)$. Its real [eigenvalues](../../../../eigenvalue.md) have opposite signs, so **$(1,1)$ is a [saddle equilibrium](../../../../saddle-equilibrium.md)**.

At $(1,2)$,

$$
M=\begin{pmatrix}4&0\\1&1\end{pmatrix},\qquad\lambda=4,1.
$$

Both [eigenvalues](../../../../eigenvalue.md) are positive, so **$(1,2)$ is an [unstable node](../../../../unstable-node.md)**.

At $(-1,1)$ the [Jacobian matrix](../../../../jacobian-matrix.md) is $\operatorname{diag}(-2,-3)$, giving **a [stable node](../../../../stable-node.md)**.

At $(-1,4)$,

$$
M=\begin{pmatrix}-8&0\\3&3\end{pmatrix},\qquad\lambda=-8,3,
$$

so **$(-1,4)$ is a [saddle equilibrium](../../../../saddle-equilibrium.md)**. All five [equilibria](../../../../equilibrium-point-of-a-dynamical-system.md) are [hyperbolic](../../../../hyperbolic-equilibrium-point.md), so these linear classifications determine their nonlinear local stability as well.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
