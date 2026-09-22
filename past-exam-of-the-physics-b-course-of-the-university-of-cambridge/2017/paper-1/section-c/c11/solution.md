<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

**Radial energy and effective potential.** For a [central force](../../../../../central-force.md) with [potential energy](../../../../../potential-energy.md) $U(r)$, [angular momentum conservation](../../../../../conservation-of-angular-momentum.md) fixes $J=mr^2\dot\phi$ and confines motion to a plane. The [kinetic energy](../../../../../kinetic-energy.md) separates into radial and angular parts, giving

$$
\boxed{E=\frac12m\dot r^2+U_{\rm eff}(r),\qquad
U_{\rm eff}(r)=U(r)+\frac{J^2}{2mr^2}.}
$$

The second term is the [centrifugal barrier](../../../../../centrifugal-barrier.md). It converts the radial motion to a one-dimensional energy problem: allowed radii have $E\geq U_{\rm eff}$, turning points have equality, and a circular orbit occurs at a stationary point of $U_{\rm eff}$. Stability of that radial orbit requires a local minimum.

**The first-order orbit equation.** Write $A=GMm$. Since $f=-dU/dr=-A/r^2-A\gamma/r^3$, choose zero potential at infinity to get

$$
U(r)=-\frac Ar-\frac{A\gamma}{2r^2},\qquad
U_{\rm eff}(r)=-\frac Ar+\frac{J^2-mA\gamma}{2mr^2}.
$$

Also $\dot r=(dr/d\phi)J/(mr^2)$. Substitute this into the energy equation and multiply by $2mr^4/J^2$:

$$
\boxed{\left(\frac{dr}{d\phi}\right)^2
-\frac{2mE}{J^2}r^4-\frac{2mA}{J^2}r^3
+\left(1-\frac{mA\gamma}{J^2}\right)r^2=0.}
$$

Here $\gamma$ has units of length. A regular bound orbit with a centrifugal barrier requires $J^2>mA\gamma$ as well as the appropriate negative energy.

**Solving in inverse radius.** Let $u=1/r$ and define

$$
q=1-\frac{mA\gamma}{J^2}>0,\qquad b=\frac{mA}{J^2}.
$$

Dividing the first-order equation by $r^4$ gives

$$
(u')^2+qu^2-2bu-\frac{2mE}{J^2}=0.
$$

Differentiating, or directly using the [Binet equation](../../../../../binet-equation.md), gives $u''+qu=b$. The continuation through turning points follows from this smooth second-order equation. Its noncircular bound solution, with angular origin at a pericentre, is

$$
u=\frac bq\left[1+e\cos(\sqrt q\,\phi)\right],\qquad
 e^2=1+\frac{2E(J^2-mA\gamma)}{mA^2},\quad0<e<1.
$$

Substitution into the first-order equation fixes the amplitude through this $e$. Therefore the requested representation holds with

$$
\boxed{\alpha_1=\frac{q}{be}
=\frac{J^2-mA\gamma}{mAe},\qquad
\alpha_2=\frac1e,\qquad
\alpha_3=\sqrt{1-\frac{mA\gamma}{J^2}},}
$$

since $\alpha_1/r-\alpha_2=\cos(\alpha_3\phi)$. A general angular origin replaces $\phi$ by $\phi-\phi_0$. This is the [orbit equation for combined inverse-square and inverse-cube attraction](../../../../../orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction.md). The circular limit $e=0$ is regular in $u=b/q$ but is not represented by finite $\alpha_1,\alpha_2$ in the source's normalized cosine form.

**Precession and the inferred length.** The last expression immediately gives

$$
\boxed{\gamma=\frac{J^2(1-\alpha_3^2)}{mA}.}
$$

Successive pericentres occur after angular advance $2\pi/\alpha_3$, so the [apsidal precession](../../../../../apsidal-precession.md) per orbit is

$$
\Delta\varpi=2\pi\left(\frac1{\alpha_3}-1\right).
$$

For $\alpha_3$ near one, $1-\alpha_3^2\simeq\Delta\varpi/\pi$. [Inferring an inverse-cube perturbation from apsidal precession](../../../../../inferring-an-inverse-cube-perturbation-from-apsidal-precession.md) consequently gives $\gamma\simeq[J^2/(mA)]\Delta\varpi/\pi$. For the stipulated nearly circular approximation, $J^2/(mA)\simeq r_0$, and [Kepler's third law](../../../../../kepler-s-third-law.md) gives

$$
r_0\simeq\left[GM\left(\frac P{2\pi}\right)^2\right]^{1/3}
\simeq5.80\times10^{10}\ \mathrm m,
$$

using $P=88(86400)\ \mathrm s$, $M=2.0\times10^{30}\ \mathrm{kg}$ and $G=6.6743\times10^{-11}\ \mathrm{m^3\,kg^{-1}\,s^{-2}}$. A century contains about $36525/88=415.1$ orbits. Convert the observed advance to radians per orbit before using it:

$$
\Delta\varpi=\frac{43}{415.1}\frac{\pi}{180(3600)}
\simeq5.02\times10^{-7}\ \mathrm{rad}.
$$

Hence

$$
\boxed{\gamma\simeq\frac{(5.80\times10^{10})(5.02\times10^{-7})}{\pi}
\simeq9.3\times10^3\ \mathrm m\simeq9.3\ \mathrm{km}.}
$$

The positive sign strengthens the attraction and gives prograde precession. The fractional perturbation $\gamma/r_0\simeq1.6\times10^{-7}$ validates the small-deviation expansion. This is the parameter fitting the proposed phenomenological [force](../../../../../force-split.md) law under the specified small-eccentricity approximation, not a derivation of that law as the physical explanation of Mercury's anomaly.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
