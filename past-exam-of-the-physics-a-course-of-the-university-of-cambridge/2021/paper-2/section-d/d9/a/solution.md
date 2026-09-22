<h1 id="section-d/d9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [metal](../../../../../../metal.md), a partially filled [energy band](../../../../../../energy-band.md) or overlapping [energy bands](../../../../../../energy-band.md) supplies [electrons](../../../../../../electron.md) with nearby unoccupied states. At [thermal equilibrium](../../../../../../thermal-equilibrium-split.md), oppositely directed [group velocities](../../../../../../group-velocity.md) are equally populated and the net [electric current](../../../../../../electric-current.md) vanishes. An applied [electric field](../../../../../../electric-field-split.md) distorts the occupation distribution, producing a small mean [drift velocity](../../../../../../drift-velocity.md). A filled [energy band](../../../../../../energy-band.md) alone has no such low-field intraband response because its velocity contributions cancel over the entire [Brillouin zone](../../../../../../brillouin-zone.md).

In the [Drude model](../../../../../../drude-model.md), let $n$ be the mobile [electron](../../../../../../electron.md) [number density](../../../../../../number-density.md), let $e>0$ be the [elementary charge](../../../../../../elementary-charge.md), and let $\tau$ be the [momentum relaxation time](../../../../../../momentum-relaxation-time.md). The mean motion obeys

$$
m\frac{d\mathbf v_d}{dt}=-e\mathbf E-\frac{m\mathbf v_d}{\tau}.
$$

The steady state is $\mathbf v_d=-e\tau\mathbf E/m$. The [current density](../../../../../../current-density.md) is opposite to the [electron](../../../../../../electron.md) [drift velocity](../../../../../../drift-velocity.md):

$$
\boxed{\mathbf J=-ne\mathbf v_d=\sigma\mathbf E,\qquad
\sigma=\frac{ne^2\tau}{m},\qquad \rho_{\rm el}=\frac{m}{ne^2\tau}.}
$$

This gives microscopic [Ohm's law](../../../../../../ohm-s-law.md), with [electrical conductivity](../../../../../../electrical-conductivity.md) $\sigma$ in $\mathrm{S\,m^{-1}}$ and [electrical resistivity](../../../../../../electrical-resistivity.md) $\rho_{\rm el}$ in $\Omega\,\mathrm m$. For a uniform wire of length $\ell$ and cross-sectional [area](../../../../../../surface-area.md) $A$, its [electrical resistance](../../../../../../electrical-resistance.md) is $R=\rho_{\rm el}\ell/A$. The dissipated [power](../../../../../../power.md) per [volume](../../../../../../volume.md) is $\mathbf J\cdot\mathbf E=\sigma E^2$, the [Joule heating](../../../../../../joule-heating.md) supplied by the external source.

The [free electron model](../../../../../../free-electron-model.md) with [Fermi-Dirac statistics](../../../../../../fermi-dirac-statistics.md) improves the microscopic picture. The [Pauli exclusion principle](../../../../../../pauli-exclusion-principle.md) fills states up to the [Fermi energy](../../../../../../fermi-energy.md) at low [temperature](../../../../../../temperature-split.md). For a spherical, parabolic [energy band](../../../../../../energy-band.md) with two [spin](../../../../../../spin.md) states,

$$
k_F=(3\pi^2n)^{1/3},\qquad E_F=\frac{\hbar^2k_F^2}{2m},\qquad v_F=\frac{\hbar k_F}{m}.
$$

Only states near the [Fermi surface](../../../../../../fermi-surface.md) change their occupation in a weak-field response; the large equilibrium [Fermi velocity](../../../../../../fermi-velocity.md) is not the small [drift velocity](../../../../../../drift-velocity.md). The same $ne^2\tau/m$ formula results for this isotropic parabolic model when $\tau$ is evaluated for transport near the [Fermi surface](../../../../../../fermi-surface.md). In a crystal, the [energy band](../../../../../../energy-band.md) [group velocity](../../../../../../group-velocity.md), [effective mass](../../../../../../band-effective-mass.md) and possibly direction-dependent scattering replace the simplest bare-particle picture. The [mean free path](../../../../../../mean-free-path.md) is approximately $\ell_{\rm mfp}=v_F\tau$.

A perfectly periodic static lattice is already included in [Bloch states](../../../../../../bloch-state.md) and does not by itself give a finite [electrical resistivity](../../../../../../electrical-resistivity.md). [Momentum](../../../../../../momentum-split.md) relaxation comes from defects, impurities, boundaries, and [electron-phonon scattering](../../../../../../electron-phonon-scattering.md). Independent scattering mechanisms approximately add their rates, giving [Matthiessen's rule](../../../../../../matthiessen-s-rule.md),

$$
\frac1\tau\simeq\frac1{\tau_{\rm imp}}+\frac1{\tau_{\rm ph}}+\cdots,\qquad
\rho_{\rm el}(T)\simeq\rho_0+\rho_{\rm ph}(T).
$$

The approximately temperature-independent $\rho_0$ is the [residual resistivity](../../../../../../residual-resistivity.md). In ordinary simple metals, the phonon contribution is approximately proportional to [temperature](../../../../../../temperature-split.md) at high [temperature](../../../../../../temperature-split.md); a three-dimensional acoustic-phonon transport model gives a $T^5$ contribution well below the relevant [Debye temperature](../../../../../../debye-temperature.md). Other mechanisms can dominate in particular materials or regimes, so neither power law is universal.

The classical [Drude model](../../../../../../drude-model.md) incorrectly treats the equilibrium carrier statistics. [Fermi-Dirac statistics](../../../../../../fermi-dirac-statistics.md) explains the small [electronic heat capacity](../../../../../../electronic-heat-capacity.md), while electrons carrying both charge and heat give the approximate [Wiedemann-Franz law](../../../../../../wiedemann-franz-law.md) $\kappa_e/(\sigma T)=\pi^2k_B^2/(3e^2)$ for degenerate carriers with appropriate nearly elastic scattering. Both the simple [electrical conductivity](../../../../../../electrical-conductivity.md) formula and this thermal relation depend on the assumptions about [energy bands](../../../../../../energy-band.md) and scattering, rather than being exact for all [metals](../../../../../../metal.md).

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D9](../../d9.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
