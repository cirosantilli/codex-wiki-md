<h1 id="section-b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**The local conservation laws.** The first equation is the radial [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md): the [material acceleration](../../../../material-acceleration.md) $Du/Dt=\partial_tu+u\partial_ru$ is caused by the [pressure gradient](../../../../pressure-gradient.md) force per unit mass, $-\partial_rp/\rho$. It neglects gravity and viscosity. The second equation is [mass conservation](../../../../mass-conservation.md) in spherical coordinates,

$$
\partial_t\rho+\frac1{r^2}\partial_r(r^2\rho u)=0.
$$

The term $2\rho u/r$ appears because the area of a spherical surface grows as $r^2$.

To obtain the third equation, let $e=p/[(\gamma-1)\rho]$ be the [specific internal energy](../../../../specific-internal-energy.md) of an [ideal gas](../../../../ideal-gas-split.md) with constant [heat capacity ratio](../../../../heat-capacity-ratio.md) $\gamma$. The [first law of thermodynamics](../../../../first-law-of-thermodynamics-split.md) for a smooth adiabatically moving element is

$$
\frac{De}{Dt}+p\frac{D(1/\rho)}{Dt}=0,
\qquad
\frac{De}{Dt}=\frac p{\rho^2}\frac{D\rho}{Dt}.
$$

Differentiating $e$ and collecting terms gives

$$
\frac{1}{(\gamma-1)\rho}\frac{Dp}{Dt}
-\frac{p}{(\gamma-1)\rho^2}\frac{D\rho}{Dt}
=\frac p{\rho^2}\frac{D\rho}{Dt},
$$

and hence

$$
\frac{Dp}{Dt}=\frac{\gamma p}{\rho}\frac{D\rho}{Dt},\qquad
\boxed{\left(\partial_t+u\partial_r\right)(p\rho^{-\gamma})=0.}
$$

Thus the entropy parameter $p/\rho^\gamma$ is conserved along each smooth [pathline](../../../../pathline.md); for fixed composition, [specific entropy](../../../../specific-entropy.md) differs from $c_v\ln(p/\rho^\gamma)$ only by a constant. This is local [isentropic flow](../../../../isentropic-flow.md) behind the shock. A physical [shock wave](../../../../shock-wave.md) itself generates [entropy](../../../../entropy-split.md) and must be treated with jump conditions, rather than by applying this smooth equation across the discontinuity.

**The front-radius scaling.** In the [self-similar blast wave](../../../../self-similar-blast-wave.md) approximation there is no scale set by ambient pressure, cooling, gravity, or the initial source radius. Write $R\propto E^a\rho_0^bt^d$. Using $[E]=\mathsf M\mathsf L^2\mathsf T^{-2}$ and $[\rho_0]=\mathsf M\mathsf L^{-3}$, [dimensional analysis](../../../../dimensional-analysis.md) gives

$$
a+b=0,\qquad 2a-3b=1,\qquad -2a+d=0.
$$

Thus $a=1/5$, $b=-1/5$, $d=2/5$ and

$$
\boxed{R=\xi_0\left(\frac E{\rho_0}\right)^{1/5}t^{2/5}.}
$$

The dimensionless coefficient $\xi_0$ depends on $\gamma$ and the resolved [similarity profiles](../../../../similarity-profile.md); dimensions alone do not fix it. Define the length scale $\ell(t)=(Et^2/\rho_0)^{1/5}$, so $\xi=r/\ell$ and the front is at the fixed coordinate $\xi=\xi_0$.

**Kinetic energy.** Substitute $\rho=\rho_0f_\rho(\xi)$ and $u=(r/t)f_u(\xi)$ into the volume integral. Since $r=\ell\xi$ and $dr=\ell\,d\xi$,

$$
E_{\rm kin}=\frac{2\pi\rho_0}{t^2}\int_0^Rr^4f_\rho f_u^2\,dr
=\frac{2\pi\rho_0\ell^5}{t^2}\int_0^{\xi_0}\xi^4f_\rho f_u^2\,d\xi.
$$

But $\rho_0\ell^5/t^2=E$, so the first of the [spherical blast-wave similarity energy integrals](../../../../spherical-blast-wave-similarity-energy-integrals.md) is

$$
\boxed{E_{\rm kin}=2\pi E\int_0^{\xi_0}\xi^4f_\rho(\xi)f_u(\xi)^2\,d\xi
=\text{constant}.}
$$

The conclusion requires a fixed, integrable [similarity profile](../../../../similarity-profile.md), as in the finite-energy blast solution. Expansion increases the swept-up mass while reducing the characteristic squared speed, leaving this product constant.

**Pressure and internal energy.** The derivatives of the [similarity variable](../../../../similarity-variable.md) are

$$
\left.\partial_t\xi\right|_r=-\frac{2\xi}{5t},\qquad
\left.\partial_r\xi\right|_t=\frac1\ell.
$$

Writing a prime for differentiation with respect to $\xi$, the [material acceleration](../../../../material-acceleration.md) becomes

$$
\partial_tu=\frac r{t^2}\left[-f_u-\frac25\xi f_u'\right],\qquad
u\partial_ru=\frac r{t^2}\left[f_u^2+\xi f_uf_u'\right],
$$



$$
\frac{Du}{Dt}=\frac r{t^2}\left[f_u^2-f_u+\xi\left(f_u-\frac25\right)f_u'\right].
$$

The radial momentum equation therefore requires a [pressure gradient](../../../../pressure-gradient.md) on the scale $\rho_0\ell/t^2$. Integrating over radius gives [pressure similarity in a spherical blast wave](../../../../pressure-similarity-in-a-spherical-blast-wave.md):

$$
\boxed{p(r,t)=\rho_0\frac{\ell^2}{t^2}f_p(\xi)
=E^{2/5}\rho_0^{3/5}t^{-6/5}f_p(\xi),}
$$

where

$$
\boxed{f_p'=-\xi f_\rho\left[f_u^2-f_u+\xi\left(f_u-\frac25\right)f_u'\right].}
$$

The prefactor has units $\mathrm{kg\,m^{-1}\,s^{-2}}$, as required for [pressure](../../../../pressure-split.md). Strictly, the momentum equation alone permits an additional pressure uniform in space and arbitrary in time. In the scale-free strong-blast solution, shock matching and the remaining thermodynamic equation fix that freedom with the same similarity scaling; any allowed constant of integration is included in $f_p$. An independently imposed external pressure would introduce another scale and invalidate the simple dimensional ansatz.

For constant $\gamma>1$, the [internal energy](../../../../internal-energy-split.md) is consequently

$$
E_{\rm int}=\frac{4\pi}{\gamma-1}\frac{\rho_0\ell^5}{t^2}
\int_0^{\xi_0}\xi^2f_p(\xi)\,d\xi,
$$



$$
\boxed{E_{\rm int}=\frac{4\pi E}{\gamma-1}\int_0^{\xi_0}\xi^2f_p(\xi)\,d\xi
=\text{constant}.}
$$

If $E$ is the total excess explosion [energy](../../../../energy-split.md), its normalization is

$$
1=2\pi\int_0^{\xi_0}\xi^4f_\rho f_u^2\,d\xi
+\frac{4\pi}{\gamma-1}\int_0^{\xi_0}\xi^2f_p\,d\xi.
$$

The two constant fractions need not be equal. No explicit solution for $f_p$ is needed to establish their time independence.

## ↑ Ancestors (13)

1. [5](../5.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
