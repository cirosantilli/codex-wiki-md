<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

In [electrostatics](../../../../../electrostatics-split.md), the [Maxwell equations in matter](../../../../../maxwell-equations-in-matter.md) are

$$
\nabla\cdot\mathbf D=\rho_f,\qquad \nabla\times\mathbf E=\mathbf0,
\qquad \mathbf D=\epsilon_0\mathbf E+\mathbf P.
$$

Here $\rho_f$ is free [charge density](../../../../../charge-density.md) and $\mathbf P$ is [polarization density](../../../../../polarization-density.md). For a homogeneous isotropic linear [dielectric](../../../../../dielectric.md), the [constitutive equation](../../../../../constitutive-equation.md) is $\mathbf D=\epsilon_0\epsilon_r\mathbf E$. Integrating the first equation over a thin pillbox straddling an interface, with unit normal $\mathbf n$ from medium 1 to medium 2, gives $\mathbf n\cdot(\mathbf D_2-\mathbf D_1)=\sigma_f$. Integrating the second around a vanishingly narrow rectangular loop gives $\mathbf n\times(\mathbf E_2-\mathbf E_1)=\mathbf0$. These are the [electrostatic interface boundary conditions](../../../../../electrostatic-interface-boundary-conditions.md). When there is no free surface [electric charge](../../../../../electric-charge-split.md), the normal [electric displacement field](../../../../../electric-displacement-field.md) and tangential [electric field](../../../../../electric-field-split.md) are continuous; the normal [electric field](../../../../../electric-field-split.md) generally is not.

Neglect end [fringing field of a capacitor](../../../../../fringing-field-of-a-capacitor.md). In either axial segment of the [coaxial cylindrical capacitor](../../../../../coaxial-cylindrical-capacitor.md), a cylindrical [Gaussian surface](../../../../../gaussian-surface.md) gives $D_r=\lambda_f/(2\pi r)$, where $\lambda_f$ is free [electric charge](../../../../../electric-charge-split.md) per length. Integrating the radial [electric field](../../../../../electric-field-split.md) between the conductors gives

$$
V=\frac{\lambda_f}{2\pi\epsilon_0\epsilon_r}\ln\frac ba,
\qquad C'=\frac{\lambda_f}{V}=\frac{2\pi\epsilon_0\epsilon_r}{\ln(b/a)}.
$$

The liquid and air segments share the same conductor [electric potential difference](../../../../../electric-potential-difference.md), so their capacitances add in parallel. Thus the [partially filled coaxial capacitor](../../../../../partially-filled-coaxial-capacitor.md) has

$$
\boxed{C(h)=\frac{2\pi\epsilon_0}{\ln(b/a)}[L-h+\epsilon h].}
$$

Here the question's $\epsilon$ is relative [permittivity](../../../../../permittivity-split.md), and air's relative [permittivity](../../../../../permittivity-split.md) is approximated by one.

Write $x$ for the rise above the external level. The wide reservoir keeps that level approximately fixed. At constant applied [voltage](../../../../../voltage.md), one must include work done by the source: the appropriate electrical contribution to the mechanical potential is $-C V^2/2$. The upward [dielectric insertion force at fixed voltage](../../../../../dielectric-insertion-force-at-fixed-voltage.md) is consequently

$$
F_e=\frac12V^2\frac{dC}{dx}
=\frac{\pi\epsilon_0(\epsilon-1)V^2}{\ln(b/a)}.
$$

The excess [hydrostatic pressure](../../../../../hydrostatic-pressure.md) $\rho gx$ acts over the annular area $A=\pi(b^2-a^2)$. Alternatively its gravitational [potential energy](../../../../../potential-energy.md) is $\rho gAx^2/2$, since liquid initially at the reservoir level must be raised through all heights from zero to $x$. Balancing the derivatives gives

$$
\boxed{x=\Delta h=\frac{\epsilon_0(\epsilon-1)V^2}{\rho g(b^2-a^2)\ln(b/a)}.}
$$

This assumes $h+x<L$, a communicating liquid reservoir, negligible capillarity, and a sufficiently long [capacitor](../../../../../capacitor.md) that end effects are small. Differentiating gives the [dielectric-rise voltmeter](../../../../../dielectric-rise-voltmeter.md)'s sensitivity at a bias $V$:

$$
\boxed{\frac{dx}{dV}=\frac{2\epsilon_0(\epsilon-1)V}{\rho g(b^2-a^2)\ln(b/a)}.}
$$

To obtain its numerical value in $\mu\mathrm m\,\mathrm V^{-1}$, multiply the right-hand side in SI units by $10^6$. A convenient parametric scale, with $\beta=b/a$, is

$$
\frac{dx}{dV}=1.805\times10^{-3}\,
\frac{\epsilon-1}{(\beta^2-1)\ln\beta}
\left(\frac V{1\ \mathrm V}\right)
\left(\frac{10^3\ \mathrm{kg\,m^{-3}}}{\rho}\right)
\left(\frac{1\ \mathrm{mm}}a\right)^2
\left(\frac{9.81\ \mathrm{m\,s^{-2}}}g\right)
\ \mu\mathrm m\,\mathrm V^{-1}.
$$

For a concrete estimate, choose $a=1\,\mathrm{mm}$, $b=2\,\mathrm{mm}$, [mass density](../../../../../density.md) $\rho=10^3\,\mathrm{kg\,m^{-3}}$, [relative permittivity](../../../../../relative-permittivity.md) $\epsilon=2$ and operating [voltage](../../../../../voltage.md) $V=100\,\mathrm V$. These are illustrative choices, not supplied apparatus data. They give

$$
\boxed{\frac{dx}{dV}\simeq0.087\,\mu\mathrm m\,\mathrm V^{-1},\qquad x\simeq4.3\,\mu\mathrm m.}
$$

Thus this millimetre-scale example requires fine optical [displacement](../../../../../displacement.md) measurement for volt-level changes. The parametric formula states exactly how the estimate changes with the chosen geometry, liquid and bias.

The displacement is quadratic in [voltage](../../../../../voltage.md), cannot distinguish its sign, and has zero first-order sensitivity at zero bias. Smaller gaps and larger [relative permittivity](../../../../../relative-permittivity.md) increase sensitivity, but capillarity, leakage, [dielectric breakdown](../../../../../dielectric-breakdown.md), temperature-dependent liquid properties, and finite available rise then limit performance. A nonconducting liquid avoids a sustained conduction load, although charging still draws [electric charge](../../../../../electric-charge-split.md) and leakage is possible. A high [voltage](../../../../../voltage.md) can give a readable displacement; a low-voltage instrument would require fine displacement measurement and careful calibration.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
