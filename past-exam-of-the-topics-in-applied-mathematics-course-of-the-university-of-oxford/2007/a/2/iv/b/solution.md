<h1 id="a/2/iv/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After an [initial layer](../../../../../../initial-layer.md) of duration $O(\epsilon)$ in slow time, $v\simeq u/(u+K)$ while $u$ changes only slightly. The reduced [substrate](../../../../../../substrate-biochemistry.md) equation is

$$
\boxed{u'\simeq\eta u-\frac{\lambda u}{u+K}
=\frac{\eta u(u-u_e)}{u+K}.}
$$

Below $u_e$ it decreases to zero; above $u_e$ it increases without bound. The exact threshold for initial $v=0$ is the intersection of the [saddle equilibrium](../../../../../../saddle-equilibrium.md)'s [stable manifold](../../../../../../stable-manifold.md) with that axis. For small $\epsilon$ it is

$$
\boxed{u_*\simeq u_e=\frac{k_2e_0}{k_0s_0}-\frac{k_{-1}+k_2}{k_1s_0}.}
$$

In dimensional initial-[substrate](../../../../../../substrate-biochemistry.md) units the leading threshold is $s_0u_*\simeq k_2e_0/k_0-(k_{-1}+k_2)/k_1$. Comparing the actual initial value $u(0)=1$ to this threshold determines its fate; the reference scale can be held fixed when varying the initial [concentration](../../../../../../concentration.md).

The initial sequestration produces an $O(\epsilon)$ correction if desired. Write the [stable manifold](../../../../../../stable-manifold.md) as $u=u_e+\epsilon\phi(v)+O(\epsilon^2)$. The invariance equation at leading order gives $\phi'(v)=F(u_e,v)/G(u_e,v)=-(1-\eta)$ and $\phi(v_e)=0$. Hence

$$
\boxed{u_*=u_e+\epsilon(1-\eta)v_e+O(\epsilon^2),}
$$

for fixed [parameters](../../../../../../parameter.md) away from degenerate limits. The positive correction reflects the [substrate](../../../../../../substrate-biochemistry.md) consumed in building complexes from the initially [enzyme](../../../../../../enzyme-split.md)-free-complex state.

The physical strip $u\geq0$, $0\leq v\leq1$ is invariant, and the off-diagonal [derivatives](../../../../../../derivative.md) are nonnegative there, so ordered initial [substrate](../../../../../../substrate-biochemistry.md) values remain ordered. There are only the attracting origin and the [saddle equilibrium](../../../../../../saddle-equilibrium.md). With [Dulac function](../../../../../../dulac-function.md) $1/u$, the divergence of the weighted vector field is $-(K-\lambda)v/u^2-(1+K/u)/\epsilon<0$, excluding [periodic orbits](../../../../../../periodic-orbit.md) in its interior. The [saddle equilibrium](../../../../../../saddle-equilibrium.md) [separatrix](../../../../../../separatrix.md) therefore gives the unique threshold on the initial axis: below it solutions tend to extinction, at it they tend to the [saddle equilibrium](../../../../../../saddle-equilibrium.md), and above it they escape to infinity. Growth is at most exponential, so this is $u\to\infty$ as time tends to infinity, not a [finite-time blowup](../../../../../../finite-time-blowup.md). This is [autocatalytic enzyme clearance with a saddle threshold](../../../../../../autocatalytic-enzyme-clearance-with-a-saddle-threshold.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [Iv](../../iv.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
