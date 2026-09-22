<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

With a positive charge magnitude e, the relaxation-time equation for electrons is $m_e^*\dot{\mathbf v}=-e\mathbf E-m_e^*\mathbf v/\tau$. Steady drift is opposite the field, $\mathbf v_d=-e\tau\mathbf E/m_e^*$, so the positive [electron mobility](../../../../../electron-mobility.md) and [electrical conductivity](../../../../../electrical-conductivity.md) are

$$
\boxed{\mu_e=e\tau/m_e^*,\qquad\mathbf j=-ne\mathbf v_d=ne\mu_e\mathbf E,\qquad
\sigma=ne^2\tau/m_e^*.}
$$

This is the weak-field [Drude model](../../../../../drude-model.md); the mobility is a magnitude, not the signed velocity-to-field ratio.

For an intrinsic nondegenerate semiconductor, $n_i=p_i=\sqrt{N_cN_v}e^{-E_g/(2k_BT)}$. Equal electron and hole masses give $N_c=N_v$ and intrinsic chemical potential midway between the band edges. At300K, the exponential is $e^{-19.34}=3.98\times10^{-9}$. Using the later supplied mass $0.015m_e$ gives

$$
N_c=2\left(\frac{m^*k_BT}{2\pi\hbar^2}\right)^{3/2}=4.61\times10^{22}\,\mathrm{m^{-3}},\qquad
\boxed{n_i\simeq1.84\times10^{14}\,\mathrm{m^{-3}}.}
$$

This is many orders below a typical metal's carrier density. Since $\sigma_i=en_i(\mu_e+\mu_h)$, ordinary finite carrier mobilities leave its intrinsic conduction negligible on a metallic scale; the gap alone does not specify an exact conductivity without the mobilities.

Under the explicitly stipulated full donor ionization, $n\simeq N_d=10^{24}\,\mathrm{m^{-3}}$ and the supplied mobility is $0.0100\,\mathrm{m^2\,V^{-1}\,s^{-1}}$. Therefore

$$
\boxed{\sigma=eN_d\mu_e=1.60\times10^3\,\mathrm{S\,m^{-1}}.}
$$

The band diagram places the intrinsic chemical potential at midgap and a shallow isolated donor level just below the conduction edge. The doped chemical potential moves upward. Quantitatively, the [degeneracy test for a fully ionized light-mass donor gas](../../../../../degeneracy-test-for-a-fully-ionized-light-mass-donor-gas.md) gives $N_d/N_c=21.7$, so a nondegenerate logarithmic chemical-potential formula is inconsistent. The parabolic-band zero-temperature estimate is $E_{F,d}-E_c=\hbar^2(3\pi^2N_d)^{2/3}/(2m^*)=0.243\,\mathrm{eV}$; its300K value is about0.241eV. The diagram accordingly shows the doped chemical potential inside the conduction band, not between an isolated donor level and the edge.

The [hydrogenic donor state](../../../../../hydrogenic-donor-state.md) scaling using the supplied hydrogen values is

$$
\boxed{E_B=\frac{m^*/m_e}{\epsilon_r^2}(13.6\,\mathrm{eV})=0.630\,\mathrm{meV},\qquad
a^*=\frac{\epsilon_r}{m^*/m_e}a_0=63.6\,\mathrm{nm}.}
$$

The binding is much smaller than $k_BT=25.9\,\mathrm{meV}$, indicating a shallow donor on the isolated-state estimate. However, the mean donor spacing is only $N_d^{-1/3}=10\,\mathrm{nm}$, well below the orbit radius. The [donor-state overlap estimate](../../../../../donor-state-overlap-estimate.md) invalidates an independent isolated-level ionization model at this concentration. Shallow binding supports abundant mobile carriers, but the [full ionization versus isolated donor occupation](../../../../../full-ionization-versus-isolated-donor-occupation.md) distinction means full ionization cannot be justified solely by comparing binding with temperature while simultaneously retaining isolated levels and a degenerate chemical potential. The conductivity above follows the question's carrier-density assumption; an overlapping impurity/conduction-band description is needed for a self-consistent microscopic account. [§9.6, donor levels and semiconductor doping; isolated-level picture distinguished here from the high-density limit](../../../../../university-physics-volume-3-by-samuel-j-ling-and-others.md)

<a id="section-c/c11/image-donor-band-reference"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-1-pa2010-donor-bands.png)

**[Figure 7](#section-c/c11/image-donor-band-reference). Donor band reference**. [Source](paper-1-pa2010-donor-bands.py). The assumed density is degenerate; the isolated donor line is a reference, not an independent-level model.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
