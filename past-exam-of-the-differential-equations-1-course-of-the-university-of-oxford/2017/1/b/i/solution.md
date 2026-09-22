<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Intersect the [nullclines](../../../../../nullcline.md) $y=x(2-x)$ and $y=kx$. Their intersection equation is $x(2-k-x)=0$, giving the origin and $(2-k,k(2-k))$. The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
M(x,y)=\begin{pmatrix}2-2x&-1\\-k&1\end{pmatrix}.
$$

At the origin, $\operatorname{tr}M=3$, $\det M=2-k$ and

$$
\lambda_\pm=\frac{3\pm\sqrt{1+4k}}2.
$$

For **$k>2$**, only the origin is in the nonnegative quadrant, and it is a **saddle** because its determinant is negative. For **$0<k<2$**, the origin is an **unstable node**, with two distinct positive [eigenvalues](../../../../../eigenvalue.md), and there is a second equilibrium in the open quadrant. At that second equilibrium, $\det M=k-2<0$, so it is a **saddle**. These signs give [hyperbolic equilibria](../../../../../hyperbolic-equilibrium-point.md), so the nonlinear classifications follow from the [linearization stability theorem](../../../../../linearization-stability-theorem.md). The boundary value $k=2$ is excluded from the two stated cases.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
