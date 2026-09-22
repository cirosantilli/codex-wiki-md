<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a [metal](../../../../../../metal.md), mobile [electrons](../../../../../../electron.md) transport heat as well as electric charge. A [temperature](../../../../../../temperature-split.md) gradient creates an imbalance between carriers arriving from warmer and colder regions. The resulting [heat current](../../../../../../heat-current.md) obeys [Fourier's law](../../../../../../fourier-s-law.md) $\mathbf j_Q=-\kappa\nabla T$ for an isotropic material, where [thermal conductivity](../../../../../../thermal-conductivity.md) $\kappa$ has units $\mathrm{W\,m^{-1}\,K^{-1}}$. For a bar of area $A$ carrying steady heat flow $P$, $P=-\kappa A\,dT/dx$ when parasitic losses are negligible.

A kinetic estimate for the electronic contribution is

$$
\kappa_e\simeq\frac13 C_ev_F\ell_\kappa=\frac13C_ev_F^2\tau_\kappa,
$$

where $C_e$ is the [electronic heat capacity](../../../../../../electronic-heat-capacity.md) per volume, $v_F$ the [Fermi velocity](../../../../../../fermi-velocity.md), and $\ell_\kappa=v_F\tau_\kappa$ the heat-transport mean free path. [Fermi-Dirac statistics](../../../../../../fermi-dirac-statistics.md) and the [Pauli exclusion principle](../../../../../../pauli-exclusion-principle.md) restrict thermal rearrangements to states near the [Fermi surface](../../../../../../fermi-surface.md), rather than allowing every [electron](../../../../../../electron.md) to contribute a classical heat capacity. A degenerate parabolic band gives

$$
C_e=\frac{\pi^2nk_B^2T}{2E_F},\qquad
\boxed{\kappa_e=\frac{\pi^2nk_B^2T\tau_\kappa}{3m}.}
$$

Using the [Drude model](../../../../../../drude-model.md) form $\sigma=ne^2\tau_\sigma/m$ for electrical transport, the relation between [thermal and electrical relaxation times in metals](../../../../../../thermal-and-electrical-relaxation-times-in-metals.md) becomes

$$
\frac{\kappa_e}{\sigma T}=\frac{\pi^2}{3}\left(\frac{k_B}{e}\right)^2\frac{\tau_\kappa}{\tau_\sigma}.
$$

For scattering that relaxes heat and charge currents similarly, $\tau_\kappa\simeq\tau_\sigma$ and the [Wiedemann-Franz law](../../../../../../wiedemann-franz-law.md) follows:

$$
\boxed{\frac{\kappa_e}{\sigma T}\simeq L_0,\qquad
L_0=\frac{\pi^2k_B^2}{3e^2}\simeq2.44\times10^{-8}\,\mathrm{W\,\Omega\,K^{-2}}.}
$$

Thus good electrical conductors are usually good thermal conductors. The correct quantum [Lorenz number](../../../../../../lorenz-number.md) differs from a naive classical electron-gas estimate.

Scattering from impurities, boundaries and [phonons](../../../../../../phonon.md) limits the heat-transport path. In an impurity-dominated low-temperature regime with approximately constant relaxation time, $\kappa_e$ is approximately proportional to $T$. Where phonon-limited [electrical resistivity](../../../../../../electrical-resistivity.md) is proportional to $T$ and the Wiedemann-Franz approximation is applicable, $\kappa_e$ can be roughly [temperature](../../../../../../temperature-split.md) independent. Inelastic processes can relax heat and charge currents differently, so the Lorenz ratio is not universal at all temperatures. Lattice [phonons](../../../../../../phonon.md) add a separate positive thermal contribution; the measured total is $\kappa=\kappa_e+\kappa_{\rm ph}$, and the electronic Wiedemann-Franz expression should not be applied blindly to that total.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
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
