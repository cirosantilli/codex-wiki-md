<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) equations are $x(1+x-2y)=0$ and $(x-1)y=0$. If $x=0$, the second equation gives $y=0$. Otherwise either $y=0$, giving $x=-1$, or $x=1$, giving $y=1$. Thus there are exactly three equilibria. The Jacobian is

$$
J(x,y)=\begin{pmatrix}1+2x-2y&-2x\\y&x-1\end{pmatrix}.
$$

At $(0,0)$ it is $\operatorname{diag}(1,-1)$: **a [saddle](../../../../saddle-equilibrium.md)**. At $(-1,0)$ it is $\begin{pmatrix}-1&2\\0&-2\end{pmatrix}$, with [eigenvalues](../../../../eigenvalue.md) $-1,-2$: **a [stable node](../../../../stable-node.md)**. At $(1,1)$ it is $\begin{pmatrix}1&-2\\1&0\end{pmatrix}$, with [characteristic polynomial](../../../../characteristic-polynomial.md) $\lambda^2-\lambda+2$ and [eigenvalues](../../../../eigenvalue.md) $(1\pm i\sqrt7)/2$: **an [unstable spiral](../../../../unstable-spiral.md)**. All three are hyperbolic, so the nonlinear local classifications follow from [linearization](../../../../linearization.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
