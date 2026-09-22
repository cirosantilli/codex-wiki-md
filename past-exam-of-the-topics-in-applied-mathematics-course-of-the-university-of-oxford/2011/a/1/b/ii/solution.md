<h1 id="a/1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are

$$
(0,0),\qquad(1,0),\qquad\left(\frac1\beta,1-\frac1\beta\right).
$$

The third is biologically interior only for $\beta>1$, and coincides with $(1,0)$ at $\beta=1$. The [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}r(1-2u-v)&-ru\\-\beta v&1-\beta u\end{pmatrix}.
$$

At $(0,0)$ the [eigenvalues](../../../../../../eigenvalue.md) are $r,1$, so it is a repelling node. At $(1,0)$ they are $-r,1-\beta$, giving a stable node for $\beta>1$ and a saddle for $\beta<1$.

At the interior equilibrium,

$$
J_* =\begin{pmatrix}-r/\beta&-r/\beta\\-(\beta-1)&0\end{pmatrix},\qquad\det J_*=-\frac{r(\beta-1)}\beta<0,
$$

so coexistence is a saddle. The formal equilibrium with negative $v$ for $\beta<1$ is not a population state; there its trace is negative and [determinant](../../../../../../determinant.md) positive.

At $\beta=1$ the boundary equilibrium is nonhyperbolic. To determine its behavior into the positive quadrant, put $x=u-1$. A local [center manifold](../../../../../../center-manifold.md) has $x=-v+v^2/r+O(v^3)$, so $\dot v=v^2+O(v^3)>0$ for small positive $v$. Thus it is unstable to introduction of species $v$, though attracting along the $v=0$ axis. The boundary/interior branches undergo a [transcritical bifurcation](../../../../../../transcritical-bifurcation.md) at this parameter.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
