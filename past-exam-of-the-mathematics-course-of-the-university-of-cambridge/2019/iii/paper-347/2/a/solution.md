<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $u(r)>0$ to be the inward radial speed and select the regular critical solution for a gas reservoir of density $\rho_\infty$ and [adiabatic sound speed](../../../../../../adiabatic-sound-speed.md) $c_\infty$. Other mathematically subsonic steady solutions need a different inner boundary condition. For the [polytropic equation of state](../../../../../../polytropic-equation-of-state.md), let $\gamma=1+1/n$, so

$$
c_s^2=\frac{dp}{d\rho}=\frac{n+1}{n}K\rho^{1/n},
\qquad
h=\int\frac{dp}{\rho}=(n+1)K\rho^{1/n}=nc_s^2.
$$

[Mass conservation](../../../../../../mass-conservation.md) and the [Bernoulli equation](../../../../../../bernoulli-equation.md) give

$$
\dot M=4\pi r^2\rho u,\qquad
\frac{u^2}{2}+nc_s^2-\frac{GM_{\rm BH}}r=nc_\infty^2.
$$

The gas is at rest at infinity, so its kinetic and gravitational terms vanish there.

Differentiate these two conserved quantities, using $d\log\rho/dr=-2/r-u'/u$. Eliminating the density derivative yields the polytropic [Bondi accretion](../../../../../../bondi-accretion.md) equation

$$
\left(u-\frac{c_s^2}{u}\right)\frac{du}{dr}
=\frac{2c_s^2}r-\frac{GM_{\rm BH}}{r^2}.
$$

At a regular [sonic point](../../../../../../sonic-point.md), both sides vanish:

$$
u_c=c_c,\qquad r_c=\frac{GM_{\rm BH}}{2c_c^2}.
$$

The [Bernoulli equation](../../../../../../bernoulli-equation.md) at that point reduces to $nc_\infty^2=(n-3/2)c_c^2$. For $n>3/2$, equivalently $1<\gamma<5/3$,

$$
\boxed{c_c^2=\frac{2n}{2n-3}c_\infty^2
=\frac{2c_\infty^2}{5-3\gamma},\qquad
r_c=\frac{2n-3}{4n}\frac{GM_{\rm BH}}{c_\infty^2}.}
$$

Since $c_s^2\propto\rho^{1/n}$, the critical density is $\rho_c=\rho_\infty[2n/(2n-3)]^n$. Evaluate the conserved [mass accretion rate](../../../../../../mass-accretion-rate.md) at the [sonic point](../../../../../../sonic-point.md):

$$
\boxed{\dot M_B=\frac{\pi G^2M_{\rm BH}^2\rho_\infty}{c_\infty^3}
\left(\frac{2n}{2n-3}\right)^{n-3/2}
=4\pi\lambda(\gamma)\frac{G^2M_{\rm BH}^2\rho_\infty}{c_\infty^3},}
$$

where

$$
\lambda(\gamma)=\frac14
\left(\frac{2}{5-3\gamma}\right)^{(5-3\gamma)/[2(\gamma-1)]}.
$$

The isothermal limit $\gamma\to1$ gives $\lambda=e^{3/2}/4$, agreeing with [Isothermal Bondi accretion](../../../../../../isothermal-bondi-accretion.md).

For $\gamma=5/3$, $n=3/2$ and the Newtonian critical radius tends to zero while $c_c$ diverges. The limiting critical solution approaches [Mach number](../../../../../../mach-number.md) one only as $r\to0$; it has no finite-radius Newtonian sonic transition. This is a failure of the Newtonian inner approximation, not an obstruction to accretion onto a [black hole](../../../../../../black-hole.md). A physical [Schwarzschild black hole](../../../../../../schwarzschild-spacetime.md) has a finite [event horizon](../../../../../../event-horizon.md), and the regular relativistic inflow becomes supersonic outside it.

The singular-looking factor in the rate has a finite limit. Writing $\epsilon=n-3/2$, its logarithm is $\epsilon\log[n/\epsilon]\to0$, so the [critical Bondi accretion rate for gamma equals five thirds](../../../../../../critical-bondi-accretion-rate-for-gamma-equals-five-thirds.md) is

$$
\boxed{\dot M_{B,5/3}=\frac{\pi G^2M_{\rm BH}^2\rho_\infty}{c_\infty^3}
\quad(\lambda=1/4).}
$$

This is also the leading cold-reservoir limit of [relativistic spherical accretion](../../../../../../relativistic-spherical-accretion.md); an exact rate for relativistically hot gas requires the relativistic equations, not this Newtonian expression.

For completeness, the finite relativistic [sonic point](../../../../../../sonic-point.md) can be seen without assigning it an arbitrary inner radius. Let $b=c_s^2/c^2$ denote the relativistic squared sound speed and $g=\gamma-1$. For an isentropic relativistic gas with $p=K\rho_{\rm rest}^{\gamma}$, its dimensionless [specific enthalpy](../../../../../../specific-enthalpy.md) is $h=g/(g-b)$. Conservation of rest-mass flux and relativistic Bernoulli energy gives the critical relations

$$
r_c=\frac{GM_{\rm BH}}{c^2}\frac{1+3b_c}{2b_c},
\qquad
(g-b_c)\sqrt{1+3b_c}=g-b_\infty.
$$

For $g=2/3$ and $c_\infty\ll c$, expansion gives $b_\infty\simeq(9/4)b_c^2$, hence

$$
\boxed{r_c\simeq\frac{3GM_{\rm BH}}{4cc_\infty}>\frac{2GM_{\rm BH}}{c^2}.}
$$

Here the asymptotic relativistic and Newtonian sound speeds agree to leading order. This finite-radius transition explains why the gas can reach the horizon despite the Newtonian $r_c=0$ result.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
