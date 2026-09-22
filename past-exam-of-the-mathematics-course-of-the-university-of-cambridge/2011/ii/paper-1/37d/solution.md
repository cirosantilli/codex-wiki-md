<h1 id="37d/solution">Solution</h1>

↑ **Parent:** [37D](../37d.md)

Using the affine parameter and the normalization requested for the [geodesic Lagrangian](../../../../../geodesic-lagrangian.md),

$$
\boxed{L=-2\dot u\dot v+\dot x^2+\dot y^2-2H(u,x,y)\dot u^2.}
$$

The coordinate $v$ is cyclic. Its [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) gives $\ddot u=0$. The transverse coordinate equations give $\ddot x+H_x\dot u^2=0$ and $\ddot y+H_y\dot u^2=0$. For the remaining coordinate,

$$
\frac{\partial L}{\partial\dot u}=-2\dot v-4H\dot u,\qquad\frac{\partial L}{\partial u}=-2H_u\dot u^2.
$$

Its Euler-Lagrange equation, after using $\ddot u=0$, is

$$
\boxed{\ddot u=0,\quad\ddot x+H_x\dot u^2=0,\quad\ddot y+H_y\dot u^2=0,\quad\ddot v+2(H_x\dot x+H_y\dot y)\dot u+H_u\dot u^2=0.}
$$

Compare with $\ddot x^a+\Gamma^a_{bc}\dot x^b\dot x^c=0$. With indices $(1,2,3,4)=(u,v,x,y)$, the complete list of nonzero [Christoffel symbols](../../../../../christoffel-symbol.md), including symmetry of the lower indices, is

$$
\boxed{\Gamma^2_{11}=H_u,\quad\Gamma^2_{13}=\Gamma^2_{31}=H_x,\quad\Gamma^2_{14}=\Gamma^2_{41}=H_y,\quad\Gamma^3_{11}=H_x,\quad\Gamma^4_{11}=H_y.}
$$

All contracted symbols $\Gamma^d_{ad}$ vanish. For $R_{11}$, the first derivative term in the supplied [Ricci tensor](../../../../../ricci-tensor.md) formula is $\partial_vH_u+\partial_xH_x+\partial_yH_y=H_{xx}+H_{yy}$, since $H$ is independent of $v$. The second derivative term vanishes because the trace symbols vanish. The third term vanishes for the same reason, and every possible product in the last term requires a zero symbol with upper index $1$ or a lower $2$, so it also vanishes. Thus

$$
\boxed{R_{uu}=H_{xx}+H_{yy},\qquad R_{ab}=0\text{ for the other components}.}
$$

The [Vacuum Einstein equations](../../../../../vacuum-einstein-equations.md) with zero cosmological constant require $R_{ab}=0$, and therefore $\boxed{H_{xx}+H_{yy}=0}$. The wave profile of this [plane-fronted gravitational wave](../../../../../plane-fronted-gravitational-wave.md) is harmonic in the transverse plane for each fixed $u$.

## ↑ Ancestors (11)

1. [37D](../37d.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
