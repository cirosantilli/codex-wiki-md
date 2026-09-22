<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [optimization Lagrangian](../../../../../optimization-lagrangian.md)

$$
L=x^TAx+y^TBy-\lambda(\mathbf1^Tx+\mathbf1^Ty-1).
$$

Symmetry gives the [gradient](../../../../../gradient.md) equations $2Ax=\lambda\mathbf1$ and $2By=\lambda\mathbf1$. The [positive-definite matrices](../../../../../positive-definite-matrix.md) are invertible, so define

$$
D=\mathbf1^TA^{-1}\mathbf1+\mathbf1^TB^{-1}\mathbf1>0.
$$

The affine constraint gives $\lambda=2/D$, hence

$$
\boxed{x_* =\frac{A^{-1}\mathbf1}{D},\qquad
 y_* =\frac{B^{-1}\mathbf1}{D},\qquad f_* =\frac1D.}
$$

For a global certificate, write any other feasible point as $(x_*+u,y_*+v)$. Feasibility implies $\mathbf1^Tu+\mathbf1^Tv=0$. Expansion cancels the cross terms and leaves

$$
f(x_*+u,y_*+v)-f(x_*,y_*)=u^TAu+v^TBv.
$$

By positive definiteness this is positive unless $u=v=0$. Thus the solution is the **unique [global minimum](../../../../../global-minimum.md)**, not merely a [stationary point](../../../../../stationary-point.md). This is a two-block instance of [positive quadratic minimization under one affine constraint](../../../../../positive-quadratic-minimization-under-one-affine-constraint.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
