<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use [linearization](../../../../../../linearization.md) around [Minkowski spacetime](../../../../../../minkowski-spacetime.md) after constant rescaling of $x,y$: set $A=1+\varepsilon a(u)$, $B=1+\varepsilon b(u)$, $u=t-z$. To first order,

$$
g=\eta+2\varepsilon a(u)\,dx^2+2\varepsilon b(u)\,dy^2+O(\varepsilon^2),\qquad a''+b''=0.
$$

Hence $s=a+b$ is affine in $u$, while $h=a-b$ is the freely propagating profile. The [affine transverse trace in a diagonal linearized plane wave is pure gauge](../../../../../../affine-transverse-trace-in-a-diagonal-linearized-plane-wave-is-pure-gauge.md): it has zero linearized curvature and is locally a coordinate artifact. To see this without imposing extra boundary conditions, use a first-order [linearized coordinate gauge transformation](../../../../../../linearized-coordinate-gauge-transformation.md) $h_{\mu\nu}\mapsto h_{\mu\nu}-\partial_\mu\xi_\nu-\partial_\nu\xi_\mu$, with

$$
\xi_x=\frac{\varepsilon s x}{2},\quad \xi_y=\frac{\varepsilon s y}{2},\quad \xi_t=-\frac{\varepsilon s'(x^2+y^2)}4,\quad \xi_z=\frac{\varepsilon s'(x^2+y^2)}4.
$$

The $tx,ty,zx,zy$ changes cancel and the remaining time/longitudinal changes are proportional to $s''=0$. The transverse perturbation becomes

$$
\boxed{h_{xx}=\varepsilon h(t-z),\qquad h_{yy}=-\varepsilon h(t-z),\qquad h_{xy}=0,}
$$

with all time and longitudinal components zero. It is a [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md) plane [gravitational wave](../../../../../../gravitational-wave.md) travelling in the positive $z$-direction, with [plus polarization](../../../../../../plus-polarization.md) and no [cross polarization](../../../../../../cross-polarization.md) in these transverse axes.

For freely falling nearby particles, [geodesic deviation](../../../../../../geodesic-deviation.md) gives opposite transverse tidal accelerations, since $R_{txtx}=-\varepsilon a''$ and $R_{tyty}=-\varepsilon b''=+\varepsilon a''$ in vacuum. Thus the transverse [geodesic deviation](../../../../../../geodesic-deviation.md) [eigenvalues](../../../../../../eigenvalue.md) have opposite signs; the stretching and compressing roles interchange when the [curvature](../../../../../../curvature.md) profile changes sign. If $h''=0$ as well, there is no linearized tidal wave: that special profile is also locally flat to this order. The exact diagonal metric describes a fixed transverse polarization through its opposite vacuum curvature eigenvalues; the linearized calculation identifies it as plus relative to the chosen axes.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
