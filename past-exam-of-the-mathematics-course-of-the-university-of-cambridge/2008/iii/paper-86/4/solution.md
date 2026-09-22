<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First solve the hinted fixed-gap problem. Let $y$ measure distance across the gap and $H(x)=h+x^2/(2a)$ be its leading local height. The [lubrication approximation](../../../../../lubrication-theory.md) gives $\mu u_{yy}=p_x$, with $u=0$ at $y=0,H$, so

$$
u=-\frac{p_x}{2\mu}y(H-y),\qquad q=\int_0^H u\,dy=-\frac{H^3p_x}{12\mu}.
$$

The constant flux per unit transverse length is $q$. Integrating its [pressure](../../../../../pressure.md) [gradient](../../../../../gradient.md) gives the [pressure-driven flux through a parabolic lubrication gap](../../../../../pressure-driven-flux-through-a-parabolic-lubrication-gap.md):

$$
\Delta p=12\mu q\int_{-\infty}^{\infty}\frac{dx}{(h+x^2/(2a))^3}.
$$

With $x=\sqrt{2ah}\,t$, the [integral](../../../../../integral.md) is $\sqrt{2a}\,h^{-5/2}\int_{-\infty}^{\infty}(1+t^2)^{-3}dt$. The substitution $t=\tan\chi$ gives $\int_{-\pi/2}^{\pi/2}\cos^4\chi\,d\chi=3\pi/8$, and therefore

$$
\boxed{\Delta p=\frac{9\pi\mu q\sqrt{2a}}{2h^{5/2}}.}
$$

Now take the [sphere](../../../../../sphere.md) speed to be $U>0$ downwards and assume zero net liquid through-flow, so the displaced liquid must pass through the annular gap. Near the equator, the [sphere](../../../../../sphere.md)'s surface radius is $R-z^2/(2R)+\cdots$, giving $H(z)=d+z^2/(2R)$. In the [sphere](../../../../../sphere.md) frame the relative [volume flux](../../../../../volumetric-flow-rate.md) is $U\pi(R+d)^2$; dividing by circumference $2\pi R$ gives $q\simeq UR/2$. The Couette contribution from the moving tube wall is only order $Ud$, smaller by $d/R$, so the fixed-gap [pressure](../../../../../pressure.md) result gives

$$
\Delta p\simeq\frac{9\pi\mu UR\sqrt{2R}}{4d^{5/2}}.
$$

The [pressure](../../../../../pressure.md) changes principally within axial distance $\sqrt{Rd}$ around the equator. It is nearly constant on each hemisphere, so its leading [force](../../../../../force.md) is the [pressure](../../../../../pressure.md) difference times projected area, $F_p\simeq\pi R^2\Delta p$. Direct viscous shear contributes a relative order $d/R$ and is smaller. Balance with the buoyant weight:

$$
\frac{4\pi R^3}{3}\Delta\rho g\simeq\pi R^2\frac{9\pi\mu UR\sqrt{2R}}{4d^{5/2}}.
$$

Thus the [settling speed of a nearly occluding sphere without through-flow](../../../../../settling-speed-of-a-nearly-occluding-sphere-without-through-flow.md) is

$$
\boxed{U\sim\frac{8\sqrt2\,\Delta\rho g d^2}{27\pi\mu}\left(\frac dR\right)^{1/2}.}
$$

The printed speed lacks the factor $1/\pi$. The parabolic-gap [integral](../../../../../integral.md) above fixes the normalization: its $3\pi/8$ cannot be dropped. With standard [dynamic viscosity](../../../../../dynamic-viscosity.md) and [Stokes drag law](../../../../../stokes-s-law.md) conventions, **the requested coefficient must be corrected by dividing the printed expression by $\pi$**. Also, the bypass result assumes no net through-flow; allowing a piston-like displacement of the entire fluid column would require specifying tube end conditions and a different resistance balance.

A [sphere](../../../../../sphere.md) of radius $d$ in an unbounded fluid has sedimentation speed $U_d=2\Delta\rho gd^2/(9\mu)$. Therefore

$$
\boxed{\frac U{U_d}\sim\frac{4\sqrt2}{3\pi}\left(\frac dR\right)^{1/2}\ll1.}
$$

The large confined [sphere](../../../../../sphere.md) falls much more slowly even than this much smaller unconfined [sphere](../../../../../sphere.md).

For radial offset $e<d$, let $\epsilon=e/d$. To leading order the narrowest gap varies as $d(\phi)=d(1+\epsilon\cos\phi)$. All circumferential strips share the same [pressure](../../../../../pressure.md) drop and act as parallel channels. Inverting the gap-resistance formula shows that each carries flux proportional to $d(\phi)^{5/2}\Delta p$. At fixed buoyant load, the leading [pressure](../../../../../pressure.md) drop is fixed, so the speed ratio is

$$
\boxed{\frac{U(e)}{U(0)}\simeq\frac1{2\pi}\int_0^{2\pi}(1+\epsilon\cos\phi)^{5/2}d\phi>1\quad(0<\epsilon<1).}
$$

The [eccentricity increases narrow-gap bypass mobility](../../../../../eccentricity-increases-narrow-gap-bypass-mobility.md) result holds because the gain through the wider side outweighs the loss through the narrower side. Strict [convexity](../../../../../convex-function.md) of $x^{5/2}$ and the zero mean of cosine prove the inequality. Pairing the positive- and negative-cosine contributions in the derivative proves monotonicity with offset. The broader hint's assertion for every exponent $\alpha>0$ is not correct for $0<\alpha<1$, when [concavity](../../../../../concave-function.md) reverses the inequality; the required exponent $5/2$ is in the valid convex range.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
