<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the inward radial [velocity](../../../../../velocity.md) as $u_R=-v(R)$, with $v>0$. Steady spherical [mass conservation](../../../../../mass-conservation.md) and the radial [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) give

$$
\boxed{\dot M=4\pi R^2\rho v=\text{constant}>0,\qquad vv'=-\frac1\rho p'-\Phi'.}
$$

For a [barotropic fluid](../../../../../barotropic-fluid.md), define the [sound speed](../../../../../speed-of-sound.md) $c_s^2=dp/d\rho>0$ and the [barotropic enthalpy function](../../../../../barotropic-enthalpy-function.md) by $dh=dp/\rho$. Choosing $\Phi(\infty)=0$, integration gives the [Bernoulli equation](../../../../../bernoulli-equation.md)

$$
\frac{v^2}{2}+h(\rho)+\Phi=h(\rho_\infty),\qquad p(\rho_\infty)=p_0.
$$

The continuity equation gives $\rho'/\rho=-2/R-v'/v$. Eliminating [mass density](../../../../../density.md) from the momentum equation produces the [barotropic spherical accretion equation](../../../../../barotropic-spherical-accretion-equation.md)

$$
\boxed{\left(v-\frac{c_s^2}{v}\right)v'=\frac{2c_s^2}{R}-\Phi'.}
$$

The [sonic point](../../../../../sonic-point.md) is where the inward [Mach number](../../../../../mach-number.md) $v/c_s$ equals one. A smooth solution cannot cross the vanishing coefficient on the left with a nonzero right-hand side, so a regular sonic radius must obey

$$
v_s=c_{s,s},\qquad c_{s,s}^2=\frac{R_s\Phi'(R_s)}2.
$$

Conversely a continuous flow that is subsonic at infinity and supersonic inward must cross unit [Mach number](../../../../../mach-number.md); smooth passage selects a simultaneous zero of the two sides, hence a regular [sonic point](../../../../../sonic-point.md). The associated critical accretion branch, rather than an arbitrary subsonic solution with smaller flux, is selected by these outer and inner requirements.

For the [polytropic equation of state](../../../../../polytropic-equation-of-state.md), set $\Gamma=1+1/m$ to distinguish its exponent from any separately specified perturbation exponent. Assume $K>0$ and first take the usual positive index $m>0$. Then

$$
c_s^2=\Gamma K\rho^{1/m},\qquad h=mc_s^2,\qquad \rho_\infty=(p_0/K)^{m/(m+1)},\qquad c_\infty^2=\Gamma p_0/\rho_\infty.
$$

For the attractive mixed potential, assume $\lambda,\mu>0$. The sonic condition and [Bernoulli equation](../../../../../bernoulli-equation.md) give

$$
c_{s,s}^2=\frac\lambda{R_s^2}+\frac\mu{2R_s},\qquad (m+\tfrac12)c_{s,s}^2-\frac\lambda{R_s^2}-\frac\mu{R_s}=mc_\infty^2.
$$

Hence [polytropic accretion in a mixed inverse-power potential](../../../../../polytropic-accretion-in-a-mixed-inverse-power-potential.md) reduces to

$$
mc_\infty^2R_s^2-\frac{2m-3}{4}\mu R_s-\frac{2m-1}{2}\lambda=0.
$$

For $0<m\leq1/2$ all nonzero coefficients in the left side are nonnegative for $R_s>0$, with at least one strictly positive: there is no finite positive root. For $m>1/2$ the constant term is negative and the leading coefficient positive, giving exactly one positive root. Define $B=(2m-3)\mu/4$ and $C=(2m-1)\lambda/2$. Then

$$
\boxed{m>\tfrac12\quad(1<\Gamma<3),\qquad R_s=\frac{B+\sqrt{B^2+4mc_\infty^2C}}{2mc_\infty^2}.}
$$

This is the finite-radius transonic range for the two positive attractive terms.

The critical point has real distinct crossing slopes. To check this rather than just solve the sonic equalities, put $U=\lambda/R_s^2$, $V=\mu/(2R_s)$ and $x=R_sv_s'/v_s$. Differentiating the [barotropic spherical accretion equation](../../../../../barotropic-spherical-accretion-equation.md) at its simultaneous zero gives

$$
(2m+1)x^2+4x+4+2m-m\frac{6U+4V}{U+V}=0.
$$

Its [discriminant](../../../../../discriminant.md) is $8m[2(2m-1)U+(2m-3)V]/(U+V)$. The sonic [Bernoulli equation](../../../../../bernoulli-equation.md) says $(2m-1)U+(2m-3)V=2mc_\infty^2$, so this [discriminant](../../../../../discriminant.md) is strictly positive for $m>1/2$. The accretion crossing is the slope for which $d\log(v/c_s)/d\log R<0$, namely the smaller root. The two slopes have opposite signs of this Mach-number derivative. This is the regular transonic saddle, not a singular vertical tangent.

The corresponding [mass accretion rate](../../../../../mass-accretion-rate.md) follows without an additional arbitrary [mass density](../../../../../density.md) normalization:

$$
\rho_s=\rho_\infty\left(\frac{c_{s,s}^2}{c_\infty^2}\right)^m,\qquad \boxed{\dot M=4\pi R_s^2\rho_\infty c_{s,s}\left(\frac{c_{s,s}^2}{c_\infty^2}\right)^m.}
$$

One may equivalently replace $\rho_s$ by $[c_{s,s}^2/(\Gamma K)]^m$. With a nonzero $\lambda$ term, inner free fall has $v\sim\sqrt{2\lambda}/R$ and continuity gives $\rho\propto R^{-1}$. Thus $v^2/c_s^2\propto R^{-2+1/m}$ increases without bound precisely in the positive-index range $m>1/2$, consistent with the required inner supersonic branch.

The assumptions on the parameters matter. If $\lambda=0$ and $\mu>0$, the finite sonic radius instead requires $m>3/2$, the usual [Bondi accretion](../../../../../bondi-accretion.md) range; $m=3/2$ is the zero-radius limiting critical case. If $\mu=0$ and $\lambda>0$, the condition remains $m>1/2$. With arbitrary signs of $\lambda,\mu$, one must use the quadratic and retain only positive roots with $c_{s,s}^2>0$ and real admissible crossing slopes; attraction was not explicitly given as a sign condition in the source.

If positive polytropic index was not intended as an implicit physical convention, there is a further mathematical range. For $K>0$, positive compressibility also permits $m<-1$, giving $0<\Gamma<1$. Both potential terms attractive then give a positive sonic root as well:

$$
R_s=\frac{B-\sqrt{B^2+4mc_\infty^2C}}{2mc_\infty^2}>0.
$$

The same [mass accretion rate](../../../../../mass-accretion-rate.md) formula applies; its crossing-slope [discriminant](../../../../../discriminant.md) is positive. The range $-1<m<0$ has $c_s^2<0$ and no physical acoustic sonic point, $m=-1$ has constant [pressure](../../../../../pressure.md) and zero [sound speed](../../../../../speed-of-sound.md), and $m=0$ does not define the printed equation of state. Thus the usual answer $m>1/2$ assumes $m>0$ and positive attractive coefficients; these conventions should not be confused with additional printed restrictions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
