<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

**Stabilization and screening.** [Charge stabilization of colloids](../../../../charge-stabilization-of-colloids.md) means suppressing aggregation through repulsion between similarly charged particles and their [electric double layers](../../../../electric-double-layer.md). In [DLVO theory](../../../../dlvo-theory.md), this repulsion competes with attractive [Van der Waals forces](../../../../van-der-waals-force.md). A substantial repulsive barrier compared with thermal energy $k_BT$ can make aggregation slow, even when the dispersed state is only metastable.

The [Debye–Hückel screening length](../../../../debye-huckel-screening-length.md) $\lambda_D=\kappa^{-1}$ is the characteristic range over which a weak electric potential is attenuated by rearrangement of mobile [ions](../../../../ion.md). It measures the thickness of a diffuse screening cloud, not a molecular diameter. For a plane, a weak potential decays as $e^{-\kappa x}$ into the bulk.

**Derivation and the source convention.** Put a planar interface at $x=0$, with electrolyte in $x>0$, bulk potential zero, and absolute [permittivity](../../../../permittivity-split.md) $\varepsilon=\varepsilon_0\varepsilon_r$. For a symmetric $z:z$ electrolyte, let $n_\infty$ be the bulk [number density](../../../../number-density.md) of each ionic species. The [Boltzmann distribution](../../../../boltzmann-distribution.md) gives

$$
n_\pm(x)=n_\infty\exp\left(\mp\frac{ze\psi(x)}{k_BT}\right),
$$

so the mobile [charge density](../../../../charge-density.md) is

$$
\rho_e=ze(n_+-n_-)=-2zen_\infty\sinh\left(\frac{ze\psi}{k_BT}\right).
$$

Substitution into the SI [Poisson equation](../../../../poisson-s-equation.md), $\nabla^2\psi=-\rho_e/\varepsilon$, gives the [Poisson-Boltzmann equation](../../../../poisson-boltzmann-equation.md)

$$
\nabla^2\psi=\frac{2zen_\infty}{\varepsilon}\sinh\left(\frac{ze\psi}{k_BT}\right).
$$

For $|ze\psi|\ll k_BT$, linearize the [hyperbolic sine](../../../../hyperbolic-sine.md). The [Debye–Hückel approximation](../../../../debye-huckel-approximation.md) is then

$$
\nabla^2\psi=\kappa^2\psi,\qquad
\boxed{\kappa^2=\frac{2z^2e^2n_\infty}{\varepsilon_0\varepsilon_rk_BT}\quad\text{(SI)}}.
$$

Here $z$ is the ionic valence magnitude, $e$ the elementary [electric charge](../../../../electric-charge-split.md), $k_B$ the [Boltzmann constant](../../../../boltzmann-constant.md), $T$ absolute [temperature](../../../../temperature-split.md), $\varepsilon_0$ the [vacuum permittivity](../../../../vacuum-permittivity.md), and $\varepsilon_r$ the solvent's [relative permittivity](../../../../relative-permittivity.md). For several ionic species, the numerator $2z^2e^2n_\infty$ is replaced by $e^2\sum_i z_i^2n_{i,\infty}$.

The original PDF includes an additional $4\pi$ in the denominator. That factor does not follow from SI [Poisson equation](../../../../poisson-s-equation.md) with number densities and the stated permittivities. The [Bjerrum length](../../../../bjerrum-length.md) provides a useful check: $\ell_B=e^2/(4\pi\varepsilon k_BT)$ and the consistent result is $\kappa^2=8\pi\ell_Bz^2n_\infty$. A Gaussian-unit convention moves factors of $4\pi$ together with the charge and permittivity conventions; it does not justify inserting this extra factor while retaining all the given SI quantities. Both numerical interpretations are reported below rather than silently changing the source.

**Conditions favoring stability.** Increasing the surface-potential or surface-charge magnitude usually strengthens the electrostatic barrier. Lower [ionic strength](../../../../ionic-strength.md) increases $\lambda_D$ and generally makes repulsion longer ranged; added salt and especially multivalent [counterions](../../../../counterion.md) shorten it and can promote aggregation. Suitable [pH](../../../../ph.md) can keep an ionizable surface charged, while conditions near an isoelectric state weaken charge repulsion. The solvent-dependent [Van der Waals forces](../../../../van-der-waals-force.md), charge regulation and particle geometry also affect the barrier, so a long screening length is not by itself sufficient. At fixed density and valence, the linear formula gives $\lambda_D\propto\sqrt{\varepsilon T}$, but actual temperature changes can also alter the permittivity and surface chemistry.

**Surface charge at small potential.** Take the usual one-sided planar-interface model, with negligible electric displacement on the nonaqueous side. The solution decaying into the solution is

$$
\boxed{\psi(x)=\psi_0e^{-\kappa x}}.
$$

The [electric field](../../../../electric-field-split.md) is $E_x=-\psi'=\kappa\psi_0e^{-\kappa x}$. The [electrostatic interface boundary conditions](../../../../electrostatic-interface-boundary-conditions.md) then give the [surface charge density](../../../../surface-charge-density.md)

$$
\boxed{\sigma=\varepsilon E_x(0^+)=\varepsilon\kappa\psi_0}.
$$

One can also derive it by integrating the diffuse [charge density](../../../../charge-density.md):

$$
\int_0^\infty\rho_e(x)\,dx=-\varepsilon\kappa^2\psi_0\int_0^\infty e^{-\kappa x}\,dx
=-\varepsilon\kappa\psi_0=-\sigma.
$$

Thus the diffuse layer neutralizes the surface charge. This is the [planar Debye-Hückel double layer](../../../../planar-debye-huckel-double-layer.md). If instead the object is an isolated sheet wetted by identical electrolyte on both sides, each side screens half its total charge and $\sigma_{\mathrm{sheet}}=2\varepsilon\kappa\psi_0$. The one-sided assumption is the conventional local model for the exterior of a large charged colloid; it must be stated because the question does not specify the material on the other side.

**Numerical ion density.** For $T=298.15\,\mathrm K$, $z=1$, $\kappa=10^9\,\mathrm{m^{-1}}$ and $\varepsilon=80\varepsilon_0=7.0834\times10^{-10}\,\mathrm{F\,m^{-1}}$, the consistent SI result is

$$
\boxed{n_\infty=\frac{\varepsilon k_BT\kappa^2}{2e^2}=5.68\times10^{25}\,\mathrm{m^{-3}}}.
$$

This is $\boxed{0.0943\,\mathrm{mol\,L^{-1}}}$ for each ion species, and hence also the salt concentration for a monovalent $1:1$ salt. The combined number density of both signs is $2n_\infty$.

Literal substitution into the formula printed in the PDF instead gives

$$
\boxed{n_{\infty,\mathrm{printed}}=4\pi n_{\infty,\mathrm{SI}}=7.14\times10^{26}\,\mathrm{m^{-3}}\simeq1.19\,\mathrm{mol\,L^{-1}}}.
$$

These values are distinct consequences of the source's extra factor; they cannot both describe the same physical screening length in SI with the same definition of $n_\infty$.

**Surface potential and validity.** The requested linear estimate in the one-sided model is

$$
\boxed{\psi_{0,\mathrm{linear}}=\frac{\sigma}{\varepsilon\kappa}=\frac{0.25}{(7.0834\times10^{-10})(10^9)}=0.353\,\mathrm V}.
$$

However, the [thermal voltage](../../../../thermal-voltage.md) is $k_BT/e=25.7\,\mathrm{mV}$, so $e\psi_{0,\mathrm{linear}}/(k_BT)\simeq13.7$. Thus **the small-potential approximation is not self-consistent for the supplied surface charge**. The boxed value is its formal extrapolation, not a reliable prediction of the actual surface potential.

For a valid nonlinear comparison within the ideal one-sided planar [Poisson-Boltzmann equation](../../../../poisson-boltzmann-equation.md), multiply the differential equation by $\psi'$ and use zero potential and field in the bulk. This gives

$$
(\psi')^2=\frac{8n_\infty k_BT}{\varepsilon}\sinh^2\left(\frac{e\psi}{2k_BT}\right).
$$

Using the surface boundary condition yields the [Grahame equation](../../../../grahame-equation.md) and its inverse:

$$
\sigma=\frac{2\varepsilon\kappa k_BT}{e}\sinh\left(\frac{e\psi_0}{2k_BT}\right),\qquad
\psi_0=\frac{2k_BT}{e}\operatorname{arsinh}\left(\frac{e\sigma}{2\varepsilon\kappa k_BT}\right).
$$

With the SI screening length, the latter gives $\boxed{\psi_{0,\mathrm{PB}}\simeq0.135\,\mathrm V}$. This is a nonlinear mean-field estimate under explicit assumptions, not a unique experimentally determined potential: compact interfacial layers, finite ion size and surface chemistry were not supplied. The source's normalization problem and its use of a linear formula far outside the small-potential regime are separate issues.

## ↑ Ancestors (13)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
