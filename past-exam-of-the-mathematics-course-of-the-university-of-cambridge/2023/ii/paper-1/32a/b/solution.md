<h1 id="32a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At an [equilibrium point of a dynamical system](../../../../../../equilibrium-point-of-a-dynamical-system.md), the second equation gives

$$
x(s-xy)=0.
$$

The choice $x=0$ is impossible because then $\dot x=r>0$. Hence $y=s/x$, and substitution into the first equation gives

$$
0=r-(1+s)x+sx=r-x.
$$

Thus the unique fixed point is

$$
\boxed{(x_*,y_*)=\left(r,\frac sr\right)}.
$$

Choose

$$
\boxed{\alpha=\frac r{1+s}},
$$

which satisfies $0<\alpha<r$. Let

$$
R=\left\{(x,y):x\geq\alpha,\quad 0\leq y\leq\frac s\alpha,
\quad x+y\leq r+\frac s\alpha\right\}.
$$

We check the direction of the vector field on its four edges.

On $x=\alpha$,

$$
\dot x=r-(1+s)\alpha+\alpha^2y=\alpha^2y\geq0.
$$

On $y=0$,

$$
\dot y=sx>0.
$$

On $y=s/\alpha$, where $x\geq\alpha$,

$$
\dot y=sx\left(1-\frac x\alpha\right)\leq0.
$$

Finally, throughout the system,

$$
\dot x+\dot y=r-x.
$$

On the sloping edge $x+y=r+s/\alpha$, the bound $y\leq s/\alpha$ implies $x\geq r$, and hence $\dot x+\dot y\leq0$. Every boundary edge therefore points inward. Violations of the corresponding four inequalities are driven toward the boundary in the same order, so positive trajectories enter this compact [trapping region](../../../../../../trapping-region.md) and then remain there. This is the [Brusselator trapping region](../../../../../../brusselator-trapping-region.md).

The [Jacobian matrix](../../../../../../jacobian-matrix.md) at the unique fixed point is

$$
J_*=
\begin{pmatrix}
-(1+s)+2x_*y_*&x_*^2\\
 s-2x_*y_*&-x_*^2
\end{pmatrix}
=
\begin{pmatrix}
 s-1&r^2\\
 -s&-r^2
\end{pmatrix}.
$$

Its determinant and trace are

$$
\det J_*=r^2>0,
\qquad
\operatorname{tr}J_*=s-1-r^2.
$$

When $s-1>r^2$, the trace is positive, so [linear stability of a planar equilibrium](../../../../../../linear-stability-of-a-planar-equilibrium.md) shows that the fixed point is a repeller. It lies in the interior of $R$.

Choose a trajectory in $R$ other than the equilibrium. Compactness of $R$ gives a nonempty compact omega-limit set, and the repelling equilibrium cannot belong to that set. Since there are no other equilibria, the [Poincaré-Bendixson theorem](../../../../../../poincare-bendixson-theorem.md) gives a [periodic orbit](../../../../../../periodic-orbit.md). Hence

$$
\boxed{s-1>r^2\quad\Longrightarrow\quad\text{the system has a periodic orbit}.}
$$

This is the [Brusselator periodic-orbit criterion](../../../../../../brusselator-periodic-orbit-criterion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
