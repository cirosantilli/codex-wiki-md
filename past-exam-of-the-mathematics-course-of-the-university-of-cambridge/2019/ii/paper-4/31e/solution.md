<h1 id="31e/solution">Solution</h1>

↑ **Parent:** [31E](../31e.md)

A [fixed point](../../../../../fixed-point.md) satisfies

$$
x+y^2-a=0,
\qquad
y(4x-x^2-a)=0.
$$

The branch with $y=0$ is

$$
P_0(a)=(a,0).
$$

Every other fixed point can be parametrized by its $x$-coordinate:

$$
a=4x-x^2,
\qquad
y=\pm\sqrt{x(3-x)},
\qquad 0\leq x\leq3.
$$

Equivalently,

$$
x_\pm=2\pm\sqrt{4-a},
\qquad y=\pm\sqrt{x_\pm(3-x_\pm)}.
$$

The $x_-$ pair exists for $0\leq a\leq4$, and the $x_+$ pair for $3\leq a\leq4$.

The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=
\begin{pmatrix}
1&2y\\
y(4-2x)&4x-x^2-a
\end{pmatrix}.
$$

On $P_0(a)$ its [eigenvalues](../../../../../eigenvalue.md) are $1$ and $a(3-a)$, so this branch has a [nonhyperbolic equilibrium](../../../../../nonhyperbolic-equilibrium.md) at $a=0$ and $a=3$. On a nonzero-$y$ branch,

$$
\det J=-4y^2(2-x),
$$

which vanishes at $x=2$, hence at $a=4$ and $y=\pm\sqrt2$. The three bifurcation values and locations are therefore

$$
\boxed{
\begin{array}{c|c|c}
a&\text{bifurcation locations}&\text{type suggested by the fixed-point branches}\\ \hline
0&(0,0)&\text{pitchfork},\\
3&(3,0)&\text{pitchfork},\\
4&(2,\sqrt2),(2,-\sqrt2)&\text{saddle-node at each point}.
\end{array}}
$$

For the [center manifold](../../../../../center-manifold.md) calculation, append $\dot a=0$ as in the [extended centre manifold for a parameter](../../../../../extended-centre-manifold-for-a-parameter.md).

At $(a,x,y)=(0,0,0)$ put $\mu=a$ and write the centre manifold as $x=h(y,\mu)$. Its [centre-manifold invariance equation](../../../../../centre-manifold-invariance-equation.md) is

$$
h_y\,y(4h-h^2-\mu)=h+y^2-\mu.
$$

It gives $h=\mu-y^2+O(3)$, and hence

$$
\dot y=y(4h-h^2-\mu)=3\mu y-4y^3+O(4).
$$

This is the [pitchfork bifurcation normal form](../../../../../pitchfork-bifurcation-normal-form.md) with stable nonzero centre branches for $\mu>0$: the bifurcation at $a=0$ is **supercritical**.

At $(a,x,y)=(3,3,0)$ put $u=x-3$ and $\mu=a-3$. Then

$$
\dot u=u+y^2-\mu,
\qquad
\dot y=y(-2u-u^2-\mu).
$$

Again $u=h(y,\mu)=\mu-y^2+O(3)$, so

$$
\dot y=-3\mu y+2y^3+O(4).
$$

The nonzero centre branches exist for $\mu>0$ and are unstable in the centre direction, whereas $y=0$ is centre-stable there. Thus the bifurcation at $a=3$ is a **[subcritical pitchfork bifurcation](../../../../../subcritical-pitchfork-bifurcation.md)** with reversed normal-form parameter.

Finally fix $y_0=\pm\sqrt2$ and put

$$
u=x-2,
\qquad v=y-y_0,
\qquad \mu=a-4.
$$

The translated system is

$$
\dot u=u+2y_0v+v^2-\mu,
\qquad
\dot v=-(y_0+v)(u^2+\mu).
$$

The extended centre manifold has

$$
u=-2y_0v+\mu+O(v^2,v\mu,\mu^2),
$$

and therefore

$$
\dot v=-y_0(\mu+8v^2)+O(v^3,\mu v).
$$

This is the [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md) normal form. For $\mu<0$ there are two nearby fixed points, which coalesce and disappear at $\mu=0$. The complete reductions are recorded in the [Extended centre-manifold reductions of the 2019 Cambridge reflection-symmetric system](../../../../../extended-centre-manifold-reductions-of-the-2019-cambridge-reflection-symmetric-system.md).

## ↑ Ancestors (10)

1. [31E](../31e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
