<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

Let $J_p=\int r^2dA=\pi a^4/2$ be the polar second moment of area. A twist gradient $\partial_x\theta$ gives shear strain $r\partial_x\theta$ and shear stress $Gr\partial_x\theta$. Integrating its moment over a cross section yields

$$
\boxed{C=GJ_p\frac\phi l=\frac{\pi a^4G}{2l}\phi.}
$$

The difference in torque on an element $dx$ is $GJ_p\partial_x^2\theta\,dx$, while its angular inertia is $\rho J_pdx$. Hence the [torsional wave equation in a circular shaft](../../../../../torsional-wave-equation-in-a-circular-shaft.md) is

$$
\boxed{\partial_t^2\theta=\frac G\rho\partial_x^2\theta,\qquad c_T=\sqrt{G/\rho}.}
$$

For uniform rotation at $\Omega$, transmitted power is $P=C\Omega$, so the given values give $C=100\,\mathrm{N\,m}$. The [elastic strain energy](../../../../../elastic-energy.md) and [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) are

$$
\phi=\frac{Cl}{GJ_p}=\boxed{9.95\times10^{-3}\,\mathrm{rad}},\qquad
U=\frac{C^2l}{2GJ_p}=\boxed{0.497\,\mathrm J},\qquad
K=\frac12\rho J_pl\Omega^2=\boxed{181\,\mathrm J}.
$$

The torsional transit time is $l/c_T=6.32\times10^{-4}\,\mathrm s$. If the requested maximum rates mean stored-energy-over-transit-time estimates, they are

$$
\boxed{\frac{c_TU}{l}\simeq786\,\mathrm W,\qquad\frac{c_TK}{l}\simeq286\,\mathrm{kW}.}
$$

These estimates require a physical qualification. They are not separate upper bounds on transmitted mechanical power. The exact local [energy flux of a torsional wave](../../../../../energy-flux-of-a-torsional-wave.md) is the stress-work rate

$$
\mathcal P=-GJ_p(\partial_x\theta)(\partial_t\theta).
$$

For the steadily rotating twisted shaft its magnitude is $C\Omega=30\,\mathrm{kW}$, even though this exceeds $c_TU/l$. Writing local energy densities $u_s=GJ_p\theta_x^2/2$ and $u_k=\rho J_p\theta_t^2/2$ gives $|\mathcal P|=2c_T\sqrt{u_su_k}\le c_T(u_s+u_k)$. A single travelling torsional wave has equal strain and kinetic energies; the steady shaft can instead be represented by oppositely travelling components whose powers largely cancel. Its stored strain pattern is not a fuel consumed once per transit. This distinguishes an energy-content estimate from the actual stress-mediated transport.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 2A](../../../paper-2a-split.md)
4. [2010](../../../split.md)
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

## ← Incoming links (1)

- [Solution](../../../paper-2b/section-c/c12/solution.md)
