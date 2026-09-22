<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Corotation reaches the [speed of light](../../../../speed-of-light.md) at $R_c=c/\Omega$. Extrapolating a dipole field gives $B_c\sim B_*(R_*/R_c)^3$ and [magnetic energy](../../../../magnetic-energy.md) density $\epsilon_c\sim B_c^2/\mu_0$, suppressing order-one factors. An outward [electromagnetic energy](../../../../electromagnetic-energy.md) flux of scale $\epsilon_c c$ through area of scale $R_c^2$ therefore gives

$$
\boxed{P\sim\frac{B_*^2R_*^6c}{\mu_0R_c^4}
=\frac{B_*^2R_*^6\Omega^4}{\mu_0c^3}.}
$$

This assumes a dipole-dominated field tied to the rotating star and an effective outgoing [Poynting flux](../../../../poynting-flux.md) near the [light cylinder](../../../../light-cylinder.md). The dipole extrapolation, angular pattern and surface-field convention affect the coefficient. A strictly aligned vacuum dipole would not radiate, whereas an oblique vacuum dipole does. A plasma-filled magnetosphere opens field lines and can [spin](../../../../spin.md) down even an aligned rotator, so the light-cylinder estimate is a scaling argument, not an exact vacuum emission calculation or literal rigid motion at $c$. Force-free calculations explicitly demonstrate this distinction.[abstract and spin-down luminosity versus inclination](../../../../time-dependent-force-free-pulsar-magnetospheres-axisymmetric-and-oblique-rotators-by-anatoly-spitkovsky.md)

The [energy](../../../../energy-split.md) comes primarily from [stellar rotation](../../../../stellar-rotation.md). With constant [moment of inertia](../../../../moment-of-inertia.md) $I$, $E_{\rm rot}=I\Omega^2/2$, and conservation of [energy](../../../../energy-split.md) gives $I\Omega\dot\Omega=-P$. Thus

$$
\boxed{\dot\Omega\simeq-K\Omega^3,\qquad
K=\frac{B_*^2R_*^6}{I\mu_0c^3}.}
$$

For constant $K$, differentiating gives $\ddot\Omega=-3K\Omega^2\dot\Omega$, hence $n=\Omega\ddot\Omega/\dot\Omega^2=3$. Evolving field strength, inclination, [moment of inertia](../../../../moment-of-inertia.md) or additional [torques](../../../../torque.md) invalidate the constant-$K$ prediction; generally $n=3+(\Omega/\dot\Omega)(\dot K/K)$ in this parametrization.

For radial inflow onto [mass](../../../../mass.md) $M$, take $v_{\rm ff}\sim(GM/r)^{1/2}$ and $\rho\sim\dot M/(4\pi r^2v_{\rm ff})$. [magnetic pressure](../../../../magnetic-pressure.md) decreases as $B_*^2R_*^6/(\mu_0r^6)$, while [ram pressure](../../../../ram-pressure.md) scales as $\rho v_{\rm ff}^2\propto\dot M(GM)^{1/2}r^{-5/2}$. Balancing them yields

$$
\boxed{R_M\sim\left(\frac{B_*^4R_*^{12}}{\mu_0^2GM\dot M^2}\right)^{1/7}
\propto B_*^{4/7}R_*^{12/7}\dot M^{-2/7}.}
$$

Numerical factors and disc geometry are not determined by this spherical estimate. The displayed proportionality holds $M$ fixed and requires a magnetospheric boundary outside the stellar surface.

In a disc, inflowing matter near $R_M$ has specific [angular momentum](../../../../angular-momentum.md) approximately $\sqrt{GMR_M}$. If it is transferred to a slower star, the material [torque](../../../../torque.md) is $N\sim\dot M\sqrt{GMR_M}$ and $I\dot\Omega\sim N>0$. The [corotation radius](../../../../corotation-radius.md) is $R_{\rm co}=(GM/\Omega^2)^{1/3}$, distinct from the light-cylinder radius. As stellar [spin](../../../../spin.md) approaches the inner disc's Keplerian [frequency](../../../../frequency.md), net spin-up weakens. If $R_M$ lies outside corotation, the field rotates faster than the disc and can centrifugally expel matter in the propeller regime. A characteristic equilibrium is

$$
\Omega_{\rm eq}\sim\sqrt{GM/R_M^3},\qquad
T_{\rm eq}\sim2\pi\sqrt{R_M^3/(GM)}
\propto B_*^{6/7}R_*^{18/7}\dot M^{-3/7}
$$

for fixed [mass](../../../../mass.md) and magnetic-coupling convention. A complete [magnetic torque](../../../../surface-magnetic-torque-on-an-accretion-disk.md) model can change the coefficient; a star also cannot rotate past its [mass-shedding limit](../../../../mass-shedding-limit.md), of order $\sqrt{GM/R_*^3}$.

For [opacity](../../../../opacity.md) per unit [mass](../../../../mass.md) $\kappa$, an isotropic radiative force balances gravity at $L_E=4\pi GMc/\kappa$. Efficient release of surface gravitational binding [energy](../../../../energy-split.md) gives $L_{\rm acc}\sim GM\dot M/R_*$ and therefore the [surface accretion Eddington rate](../../../../surface-accretion-eddington-rate.md)

$$
\dot M_{\max}\sim\frac{4\pi cR_*}{\kappa}\propto R_*.
$$

The radius dependence matters: it uses efficiency $\eta\sim GM/(R_*c^2)$, not an arbitrarily fixed reference efficiency. Substituting this maximal rate into the equilibrium period gives

$$
\boxed{T_{\min}\propto B_*^{6/7}R_*^{18/7}(R_*)^{-3/7}
=B_*^{6/7}R_*^{15/7}.}
$$

[mass](../../../../mass.md), [opacity](../../../../opacity.md) and geometry factors are held fixed. This is the classical radiatively efficient Eddington-limited scaling, not a universal upper bound on every [mass](../../../../mass.md) supply rate: beaming, advection, outflows and [opacity](../../../../opacity.md) changes can alter it. For sufficiently small field, $R_M\lesssim R_*$ and the magnetic scaling must be replaced by surface-disc and mass-shedding physics.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
