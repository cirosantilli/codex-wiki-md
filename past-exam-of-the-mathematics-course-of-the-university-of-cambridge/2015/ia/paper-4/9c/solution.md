<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Outside a spherical Earth the gravitational field is the field of its total mass at the center, by the [shell theorem](../../../../../spherical-shell-theorem.md). Since $GM_E=gR^2$, the [inverse-square force](../../../../../inverse-square-force.md) on the upward radial trajectory gives

$$
\boxed{\ddot z=-\frac{gR^2}{(R+z)^2},\qquad z(0)=0,\quad\dot z(0)=V.}
$$

The independent dimensional inputs are $R,V,g$, of dimensions $L,LT^{-1},LT^{-2}$. A dimensionless monomial in them must be a power of $V^2/(gR)$. Thus [dimensional analysis](../../../../../dimensional-analysis.md) gives

$$
\boxed{H=RF(\lambda),\qquad T=\frac VgG(\lambda),\qquad\lambda=\frac{V^2}{gR}.}
$$

For a finite turning height and time, assume $0<V<\sqrt{2gR}$, equivalently $0<\lambda<2$. This [escape velocity](../../../../../escape-velocity.md) restriction is implicit in the requested maximum-height formulas.

The [conservation of energy](../../../../../conservation-of-energy.md), per unit particle mass, is

$$
\frac12\dot z^2-\frac{gR^2}{R+z}=\frac12V^2-gR,
$$

so

$$
\dot z^2=V^2-\frac{2gRz}{R+z}=\frac{V^2R-(2gR-V^2)z}{R+z}.
$$

The numerator vanishes at the turning point, giving

$$
\boxed{H=\frac{V^2R}{2gR-V^2},\qquad F(\lambda)=\frac{\lambda}{2-\lambda}.}
$$

On ascent $\dot z>0$, and integrating $dt=dz/\dot z$ gives

$$
\boxed{T=\int_0^H\sqrt{\frac{R+z}{V^2R-(2gR-V^2)z}}\,dz.}
$$

The upper endpoint has an integrable inverse-square-root singularity. Set $z=Hx$, use $H=R\lambda/(2-\lambda)$ and $V^2R=(2gR-V^2)H$, and note $R\lambda/V=V/g$. The result is

$$
T=\frac Vg\int_0^1\sqrt{\frac{2-\lambda+\lambda x}{(2-\lambda)^3(1-x)}}\,dx,\qquad \boxed{G(\lambda)=\int_0^1\sqrt{\frac{2-\lambda+\lambda x}{(2-\lambda)^3(1-x)}}\,dx.}
$$

For small $\lambda$, $F(\lambda)\sim\lambda/2$ and $G(\lambda)\to1$, recovering $H\sim V^2/(2g)$ and $T\sim V/g$. At $\lambda=2$ the particle escapes marginally and has no finite maximum; for $\lambda>2$ it escapes with nonzero asymptotic speed. The finite-turning formulas must not be extended to those cases.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
