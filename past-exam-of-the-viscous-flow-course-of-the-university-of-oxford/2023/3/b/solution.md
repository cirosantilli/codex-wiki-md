<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $H(x')=h'(x')$ and $p'_x=dp'/dx'$ below, so the subscript $x$ in this shorthand denotes differentiation with respect to $x'$. The vertical [pressure gradient](../../../../pressure-gradient.md) is zero, and integrating $u'_{z'z'}=p'_x$ twice with the wall [boundary conditions](../../../../boundary-condition.md) gives the local [Couette-Poiseuille flow](../../../../couette-poiseuille-flow.md)

$$
\boxed{u'(x',z')=-1+\frac{z'}{H}
+\frac{p'_x}{2}z'(z'-H).}
$$

The first two terms are [Couette flow](../../../../couette-flow.md) due to the moving plate; the last is [plane Poiseuille flow](../../../../plane-poiseuille-flow.md) due to the local [pressure gradient](../../../../pressure-gradient.md). Its dimensionless [volume flux per unit width](../../../../volume-flux-per-unit-width.md) is

$$
q(x')=\int_0^{H(x')}u'(x',z')\,dz'
=-\frac H2-\frac{H^3}{12}\frac{dp'}{dx'}.
$$

Use the [Leibniz integral rule](../../../../leibniz-integral-rule.md) and [incompressibility](../../../../incompressible-flow.md) to differentiate this [integral](../../../../integral-split.md):

$$
\frac{dq}{dx'}=\int_0^H u'_{x'}\,dz'+u'(x',H)\frac{dH}{dx'}
=-w'(x',H)+w'(x',0)=0.
$$

Thus **the flux is independent of position**, and

$$
\boxed{\frac d{dx'}\left(\frac{H^3}{12}\frac{dp'}{dx'}+\frac H2\right)=0.}
$$

The normal [velocity](../../../../velocity.md) can then be recovered from [incompressibility](../../../../incompressible-flow.md):

$$
w'(x',z')=-\int_0^{z'}u'_{x'}(x',s)\,ds.
$$

It is zero on the lower wall by construction and zero on the upper wall by the constant-[volume flux](../../../../volumetric-flow-rate.md) relation. This supplies the remaining component of the leading [velocity field](../../../../velocity-field.md).

The endpoint [pressure](../../../../pressure-split.md) conditions are matching conditions, not an assertion that the [lubrication approximation](../../../../lubrication-theory.md) remains valid at arbitrarily large dimensional $x$. On an outer length scale $R$, a viscous [pressure](../../../../pressure-split.md) variation is of size $\mu U/R$, whose ratio to the inner scale is

$$
\frac{\mu U/R}{P}=\frac{h_0^2}{RL}=\delta^3\ll1.
$$

Even an outer inertial [pressure](../../../../pressure-split.md) scale $\rho U^2$ has ratio

$$
\frac{\rho U^2}{P}=\delta^2\mathrm{Re}\ll1.
$$

Consequently the gap [pressure](../../../../pressure-split.md) is much larger than either outer variation. Matching to fluid with a common ambient [pressure](../../../../pressure-split.md) at both ends, and taking that value as zero [gauge pressure](../../../../gauge-pressure.md), gives

$$
\boxed{p'(x')\longrightarrow0\quad(x'\to\pm\infty).}
$$

There is an [overlap region](../../../../overlap-region.md) $1\ll|x'|\ll\delta^{-1}$ before the wall slope becomes order one. The infinite endpoints represent matching through that region. An externally imposed [pressure](../../../../pressure-split.md) difference comparable with $P$ would change these conditions and the resulting [volume flux](../../../../volumetric-flow-rate.md); equal outer [pressure](../../../../pressure-split.md) is the physical assumption being used here.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the viscous flow course of the University of Oxford](../../../split.md)
5. [Viscous flow course of the University of Oxford](../../../../viscous-flow-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
