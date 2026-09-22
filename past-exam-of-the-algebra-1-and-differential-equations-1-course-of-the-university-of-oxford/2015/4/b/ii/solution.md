<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Intersect the two [nullcline](../../../../../nullcline.md) families. The axes yield $(0,0)$ and $(1,0)$, and $y=1$ with $xy=2$ yields $(2,1)$. The possible remaining intersection would have $x+y=1$ and $xy=2$, requiring $x^2-x+2=0$, whose [discriminant](../../../../../discriminant.md) is $-7$. Hence there are no further real [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md).

The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}
(1-y)(1-2x-y)&x(x+2y-2)\\
-y^2&2-2xy
\end{pmatrix}.
$$

Evaluate it at each [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md):

- At $(0,0)$ it is $\operatorname{diag}(1,2)$. Both [eigenvalues](../../../../../eigenvalue.md) are positive, so the point is an **[unstable node](../../../../../unstable-node.md)**.
- At $(1,0)$ it is $\begin{pmatrix}-1&-1\\0&2\end{pmatrix}$. The [eigenvalues](../../../../../eigenvalue.md) $-1,2$ have opposite signs, so this is a **[saddle point](../../../../../saddle-point.md)**. Its stable direction is $(1,0)$ and its unstable direction can be taken as $(-1,3)$.
- At $(2,1)$ it is $\begin{pmatrix}0&4\\-1&-2\end{pmatrix}$. Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2+2\lambda+4$, so $\lambda=-1\pm i\sqrt3$. This is an **[stable focus](../../../../../stable-spiral.md)**, or spiral sink.

All three are [hyperbolic equilibria](../../../../../hyperbolic-equilibrium-point.md), so their classifications persist for the nonlinear system. Immediately to the right of $(2,1)$ on $y=1$, the velocity is vertically downward, showing that the attracting spiral turns **clockwise**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
