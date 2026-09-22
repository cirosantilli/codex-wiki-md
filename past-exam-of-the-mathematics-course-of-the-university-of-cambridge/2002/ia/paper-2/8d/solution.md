<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Introduce $H=x^2-y^2+y^4/2$. Along a solution,

$$
\dot H=2x(\alpha x-y+y^3)+(-2y+2y^3)(-x)=\boxed{2\alpha x^2}.
$$

At $\alpha=0$, $H$ is a [first integral](../../../../../first-integral.md). The identity $H+1/2=x^2+(y^2-1)^2/2$ shows its [level sets](../../../../../level-set.md) are bounded: neither $x$ nor $y$ can escape to infinity on a fixed level. Consequently **trajectories remain bounded as $t\to\infty$**, including those starting far from the origin. This bound also prevents finite-time escape; no explicit solution is needed.

The [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are $(0,0)$ and $(0,\pm1)$. The [Jacobian matrix](../../../../../jacobian-matrix.md) at $(0,y_*)$ is

$$
J=\begin{pmatrix}\alpha&3y_*^2-1\\-1&0\end{pmatrix}.
$$

At the origin its [eigenvalues](../../../../../eigenvalue.md) are $(\alpha\pm\sqrt{\alpha^2+4})/2$, with opposite signs, so the origin is a [saddle point](../../../../../saddle-point.md) in all three cases. An [eigenvector](../../../../../eigenvector.md) for $\lambda$ lies on $y=-x/\lambda$; the stable direction has positive slope and the unstable direction negative slope. At $(0,\pm1)$ the [eigenvalues](../../../../../eigenvalue.md) are $(\alpha\pm\sqrt{\alpha^2-8})/2$.

When $\alpha=0$, these latter [eigenvalues](../../../../../eigenvalue.md) are $\pm i\sqrt2$. The nonlinear classification follows from the strict minima of $H$ at the two points: nearby [level sets](../../../../../level-set.md) are closed curves without other equilibria, and the nonvanishing vector field makes them [periodic orbits](../../../../../periodic-orbit.md). Thus the two points are [center equilibria](../../../../../center-equilibrium.md). For $-1/2<H<0$, there are two separate closed ovals, one around each [center equilibrium](../../../../../center-equilibrium.md). The level $H=0$ consists of the [saddle point](../../../../../saddle-point.md) and two [homoclinic orbits](../../../../../homoclinic-orbit.md) forming a figure eight, explicitly

$$
x=\pm y\sqrt{1-y^2/2},\qquad |y|\le\sqrt2.
$$

For $H>0$, a single outer closed orbit encloses all three [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md). Motion is clockwise, as the vector points downwards wherever $x>0$. The upper [homoclinic orbit](../../../../../homoclinic-orbit.md) leaves the origin into $x<0,y>0$ and returns through $x>0,y>0$; the lower one has the reflected orientation.

When $\alpha=0.1$, the two nonzero [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) have [eigenvalues](../../../../../eigenvalue.md) $0.05\pm i\sqrt{7.99}/2$ and are unstable [foci](../../../../../focus-dynamical-systems.md). Nearby paths spiral outward clockwise. The [first integral](../../../../../first-integral.md) becomes a strictly increasing energy along every nonconstant trajectory: although $\dot H$ can momentarily vanish when $x=0$, it cannot vanish on an interval unless the solution is an equilibrium. Thus there are no [periodic orbits](../../../../../periodic-orbit.md) or [homoclinic orbits](../../../../../homoclinic-orbit.md). The two stable separatrices of the [saddle point](../../../../../saddle-point.md), traced backwards, spiral towards the corresponding unstable [foci](../../../../../focus-dynamical-systems.md). Its unstable separatrices move onto positive energy and escape outwards. All other nonequilibrium trajectories outside the [stable manifold](../../../../../stable-manifold.md) are unbounded forwards: a bounded forward limit set would have to lie in $x=0$, whose only invariant points are the three equilibria; the two unstable [foci](../../../../../focus-dynamical-systems.md) cannot attract a nonconstant trajectory, and convergence to the saddle occurs only on its [stable manifold](../../../../../stable-manifold.md). Escape is not finite-time blow-up, since $\dot H\le2\alpha(H+1/2)$ bounds the energy on every finite interval.

When $\alpha=-0.1$, the [eigenvalues](../../../../../eigenvalue.md) at the nonzero points are $-0.05\pm i\sqrt{7.99}/2$, so they are [stable foci](../../../../../stable-spiral.md). The energy decreases, keeping all forward trajectories in compact sublevel sets. A bounded limit set must lie in the invariant part of $x=0$, so trajectories converge to equilibria: generically to one of the two [stable foci](../../../../../stable-spiral.md), exceptionally to the saddle along its [stable manifold](../../../../../stable-manifold.md). The saddle's unstable separatrices spiral into the two [stable foci](../../../../../stable-spiral.md); its [stable manifold](../../../../../stable-manifold.md) separates their attraction basins. Again, energy monotonicity excludes [periodic orbits](../../../../../periodic-orbit.md) and [homoclinic orbits](../../../../../homoclinic-orbit.md). These three cases give the [quartic double-well phase portrait with linear damping](../../../../../quartic-double-well-phase-portrait-with-linear-damping.md) below.

<a id="8d/image-conservative-double-well-closed-orbits-and-the-outward-or-inward-spirals-produced-by-positive-or-negative-alpha"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2-phase-portraits.png)

**[Figure 4](#8d/image-conservative-double-well-closed-orbits-and-the-outward-or-inward-spirals-produced-by-positive-or-negative-alpha). Conservative double-well closed orbits and the outward or inward spirals produced by positive or negative alpha**.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
