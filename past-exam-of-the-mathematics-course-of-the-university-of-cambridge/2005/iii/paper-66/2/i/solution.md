<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $U=B_0-A_0$, $T=D_0-C_0$, $D=A_0-C_0$ and $v=V-W$. A point on each moving segment has the form $A_0+sU+tV$ and $C_0+rT+tW$, with $s,r\in[0,1]$. Contact is therefore equivalent to

$$
D+sU-rT+tv=0,\qquad0\le s,r\le1,\quad t\ge0.
$$

The [contact time of translating line segments](../../../../../../contact-time-of-translating-line-segments.md) is the minimum feasible $t$. This reduces the entire continuous-motion problem to three [linear equations](../../../../../../linear-equation.md) and linear inequalities.

In three-dimensional space form the [matrix](../../../../../../matrix.md) $H=[U,-T,v]$. If it is nonsingular, solve

$$
\begin{pmatrix}s\\r\\t\end{pmatrix}=-H^{-1}D
$$

using a stable linear solver. A candidate with $s,r$ in the unit interval and $t\ge0$ is the only contact event and hence the earliest one; otherwise no contact occurs. Check initial intersection explicitly, so an already touching pair returns time zero.

If $H$ is singular, use a rank-revealing factorization to test consistency. Write every solution as $x=x_0+Nz$, with columns of $N$ spanning the [null space](../../../../../../kernel-of-a-linear-map.md), and minimize its time coordinate subject to the box and nonnegative-time constraints. This is a small [linear programming](../../../../../../linear-programming.md) problem. It handles parallel segments, collinear overlap, a continuum of contact times and segments degenerated to points. Infeasibility means no future contact. When $v=0$, the relative geometry is stationary: initially disjoint segments never meet. **The first contact is the least feasible nonnegative time, not just an intersection of the two supporting lines.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
