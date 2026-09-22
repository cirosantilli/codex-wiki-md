<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Let a one-parameter infinitesimal transformation be $\delta q_i=\epsilon X_i(q,t)$ and suppose its change in the [Lagrangian](../../../../../lagrangian.md) is a total derivative,

$$
\delta\mathcal L=\epsilon\frac{dF}{dt}.
$$

With [canonical momentum](../../../../../canonical-momentum.md) $p_i=\partial\mathcal L/\partial\dot q_i$, the chain rule and the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) give, along a motion,

$$
\delta\mathcal L
=\epsilon\sum_i\left(
\frac{\partial\mathcal L}{\partial q_i}X_i
+p_i\frac{dX_i}{dt}\right)
=\epsilon\frac d{dt}\sum_i p_iX_i.
$$

Comparison with the assumed total derivative proves [Noether theorem](../../../../../noether-theorem.md):

$$
\boxed{J=\sum_i p_iX_i-F\quad\text{is conserved}.}
$$

The given Lagrangian has no explicit time dependence, so its [energy function](../../../../../energy-function.md) is conserved:

$$
\boxed{E=\dot x\frac{\partial\mathcal L}{\partial\dot x}
+\dot y\frac{\partial\mathcal L}{\partial\dot y}-\mathcal L
=\frac{\dot x^2+\dot y^2}{2y^2}+V\!\left(\frac xy\right).}
$$

It is also invariant under the dilation $(x,y)\mapsto(e^\epsilon x,e^\epsilon y)$: the velocities and $y$ all scale by the same factor, while $x/y$ is unchanged. The generator is $(X_x,X_y)=(x,y)$ and $F=0$. Since

$$
p_x=\frac{\dot x}{y^2},
\qquad
p_y=\frac{\dot y}{y^2},
$$

Noether's theorem supplies the second first integral

$$
\boxed{D=xp_x+yp_y=\frac{x\dot x+y\dot y}{y^2}.}
$$

The integrals $E$ and $D$ are independent on an open dense subset of phase space.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
