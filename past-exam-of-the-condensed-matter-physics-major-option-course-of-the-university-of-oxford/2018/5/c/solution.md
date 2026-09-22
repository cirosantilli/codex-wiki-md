<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The displayed horizontal variable is $\mu_0H$ in tesla. The source formulas written with a flux quantum actually have the [dimensions](../../../../dimension-vector-space.md) of [magnetic flux density](../../../../magnetic-field-split.md), so define $B_{c1}=\mu_0H_{c1}$ and $B_{c2}=\mu_0H_{c2}$ when applying them:

$$
B_{c1}\simeq\frac{\Phi_0}{4\pi\lambda^2}\ln\kappa,\qquad
B_{c2}=\frac{\Phi_0}{2\pi\xi^2},\qquad\kappa=\lambda/\xi.
$$

From the onset of curvature away from the low-field line in panel A, $B_{c1}$ is roughly $0.06\,\mathrm T$ with uncertainty of order $0.01\,\mathrm T$. Panel B's branches approach the normal background over approximately $2$–$3\,\mathrm T$; use $B_{c2}\simeq2.5\,\mathrm T$ as a coarse central estimate. Resolving irreversible loop closure from the true thermodynamic upper field, and correcting demagnetization, would require better data and geometry. These readings support scales, not precise material constants.

The upper field gives

$$
\boxed{\xi=\sqrt{\frac{\Phi_0}{2\pi B_{c2}}}\simeq11.5\,\mathrm{nm}.}
$$

The [leading-log critical-field inversion](../../../../leading-log-critical-field-inversion.md) starts by dividing the two field formulas to eliminate $\xi$:

$$
\frac{B_{c1}}{B_{c2}}=\frac{\ln\kappa}{2\kappa^2}\simeq0.024.
$$

The large-$\kappa$ solution is $\kappa\simeq6.15$, hence

$$
\boxed{\lambda\simeq71\,\mathrm{nm},\qquad\xi\sim10\text{–}13\,\mathrm{nm},\quad\lambda\text{ of order }70\text{–}80\,\mathrm{nm}.}
$$

The penetration-depth range is an indicative graph/model scale, not a propagated confidence interval. There is a mathematical ambiguity worth making explicit: $f(\kappa)=\ln\kappa/(2\kappa^2)$ rises from zero at one, peaks at $\sqrt e$, then falls. The same central ratio also gives $\kappa\simeq1.055$ and $\lambda\simeq12.1\,\mathrm{nm}$, so the printed restriction $\kappa>1$ alone does not select a unique solution. The leading-log lower-field formula is intended for appreciably large $\kappa$, which motivates the $\kappa\simeq6$ branch; near one it needs the omitted core-[energy](../../../../energy-split.md) correction. Even the larger-branch estimate has systematic uncertainty from that approximation.

$\lambda$ is the [London penetration depth](../../../../london-penetration-depth.md), the magnetic screening scale, while $\xi$ is the [superconducting coherence length](../../../../superconducting-coherence-length.md), the recovery scale of the superconducting [order parameter](../../../../order-parameter.md) after spatial suppression. In the mixed state the complex [order parameter](../../../../order-parameter.md) vanishes in [vortex](../../../../phase-vortex.md) cores of radius of order $\xi$, recovers between separated cores and winds in phase by $2\pi$ around each singly quantized [vortex](../../../../phase-vortex.md). Currents and [magnetic field](../../../../magnetic-field-split.md) spread over scale $\lambda$; [vortex](../../../../phase-vortex.md) density grows with the mean internal field according to $n_v\Phi_0=\overline B$. Near $H_{c2}$ cores overlap and the order-parameter amplitude becomes small throughout the sample. A schematic core profile appears in [solution](../../3/a/solution.md).

The [hysteresis](../../../../hysteresis.md) is not the reversible equilibrium [magnetization](../../../../magnetization.md): defects pin vortices, so entry and exit leave different spatial flux distributions. Macroscopic currents oppose changes in flux, trapped vortices give remanence, and depinning and creep depend on history and [temperature](../../../../temperature-split.md). Surface barriers can also contribute. The loop width probes an irreversible current scale, but its conversion to [current density](../../../../current-density.md) additionally needs sample geometry and an appropriate critical-state model.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
