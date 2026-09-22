<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Eliminate $\dot v$ from the first equation before [linearization](../../../../linearization.md):

$$
\dot u=\mu-u-\frac\gamma\varepsilon f(u,v),\qquad
\dot v=\frac1\varepsilon f(u,v).
$$

All partial [derivatives](../../../../derivative.md) below are evaluated at $(\mu,g(\mu))$. The [Jacobian matrix](../../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}
-1-\gamma f_u/\varepsilon&-\gamma f_v/\varepsilon\\
f_u/\varepsilon&f_v/\varepsilon
\end{pmatrix}.
$$

Its [trace](../../../../matrix-trace.md) and [determinant](../../../../determinant.md) are

$$
\operatorname{tr}J=-1+\frac{f_v-\gamma f_u}{\varepsilon},\qquad
\det J=-\frac{f_v}{\varepsilon}>0.
$$

By [linear stability of a planar equilibrium](../../../../linear-stability-of-a-planar-equilibrium.md), a positive [trace](../../../../matrix-trace.md) makes both real [eigenvalues](../../../../eigenvalue.md) positive or gives a complex pair with positive real part. The [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is consequently unstable precisely when

$$
\boxed{\varepsilon-f_v<-\gamma f_u.}
$$

A negative [trace](../../../../matrix-trace.md) gives [asymptotic stability](../../../../asymptotic-stability.md); equality leaves a purely imaginary pair and requires a separate nonlinear [bifurcation](../../../../bifurcation.md) calculation. In particular, the unique positive [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is never a [saddle equilibrium](../../../../saddle-equilibrium.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
