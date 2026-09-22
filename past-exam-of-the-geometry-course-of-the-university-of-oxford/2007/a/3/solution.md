<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [critical point](../../../../critical-point.md) satisfies $df=0$; it is nondegenerate when the [Hessian](../../../../hessian-matrix.md) on its two-dimensional [tangent space](../../../../tangent-space.md) is nonsingular. For a smooth function with only nondegenerate [critical points](../../../../critical-point.md) on a compact [surface](../../../../topological-surface-split.md), the [Morse theory](../../../../morse-theory.md) formula is

$$
\boxed{\chi(X)=m_0-m_1+m_2,}
$$

where $m_i$ counts the [critical points](../../../../critical-point.md) whose [Hessian](../../../../hessian-matrix.md) has $i$ negative eigenvalues.

For $f(x)=|x|^2$, differentiation in a tangent direction $v$ gives $df_x(v)=2x\cdot v$. This vanishes for all $v\in T_xX$ exactly when the position vector is perpendicular to that [tangent plane](../../../../tangent-plane.md), equivalently the [normal line](../../../../normal-line.md) at $x$ contains the origin. This includes $x=0$, if it is on the [surface](../../../../topological-surface-split.md). On a [torus](../../../../torus.md) $\chi=0$, while a minimum and a maximum give $m_0,m_2\geq1$. Thus $m_1=m_0+m_2\geq2$ and the total is at least four. Hence **at least four [surface](../../../../topological-surface-split.md) normals pass through the origin** under the stated nondegeneracy assumption.

Write the generating circle as center $(a,R)$ and radius $r$, with $R>r>0$. A parametrization and [unit normal](../../../../unit-normal.md) are

$$
X(u,v)=(a+r\cos u,(R+r\sin u)\cos v,(R+r\sin u)\sin v),\quad n(u,v)=(\cos u,\sin u\cos v,\sin u\sin v).
$$

Take **$P=(a,R/2,0)$**. If $P-X=tn$, its first coordinate gives $(r+t)\cos u=0$. The alternative $t=-r$ would force the radial distance of $P$ from the axis to be $R$, contrary to $R/2$. Thus $\cos u=0$. The remaining equations and the nonzero radial distance of $P$ force $v=0$ or $\pi$. Each of the two choices of $u$ and two of $v$ works, giving exactly four distinct points. Take **$Q=(a,0,0)$** instead. All points on each of the circles $u=\pi/2$ and $u=3\pi/2$ have radial normals through $Q$, giving infinitely many.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
