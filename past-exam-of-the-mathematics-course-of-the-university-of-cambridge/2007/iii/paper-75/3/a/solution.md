<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Goldreich–Sridhar turbulence](../../../../../../goldreich-sridhar-turbulence.md) model in its balanced form. Assume a uniform strong guide field; anisotropic fluctuations $k_\parallel\ll k_\perp$; comparable counterpropagating [Alfvén wave](../../../../../../alfven-wave.md) amplitudes; a statistically steady [inertial range](../../../../../../inertial-range.md) with negligible forcing and dissipation within it; transfer mainly between comparable perpendicular scales; and a scale-independent [energy](../../../../../../energy.md) flux per unit mass $\mathcal E$. The estimate also assumes no extra scale-dependent alignment factor in the nonlinear interaction and neglects intermittency corrections.

Let $\ell_\perp$ and $\ell_\parallel$ be an eddy's perpendicular and parallel scales, and $\delta u_\ell\sim\delta B_\ell/\sqrt{4\pi\rho_0}$ its Alfvénic [velocity](../../../../../../velocity.md) amplitude. The nonlinear interaction is supplied by the oppositely propagating [Elsässer variable](../../../../../../elsasser-variable.md), so comparable populations give

$$
\tau_{\mathrm{nl}}\sim\frac{\ell_\perp}{\delta u_\ell}.
$$

The Alfvén propagation time is $\tau_A\sim\ell_\parallel/v_A$. For strong [turbulence](../../../../../../turbulence-split.md), [critical balance](../../../../../../critical-balance.md) makes these times comparable; the decorrelation and cascade time is therefore of order $\tau_{\mathrm{nl}}$, not a much longer time obtained by adding many weak encounters.

A constant perpendicular [energy](../../../../../../energy.md) flux gives

$$
\mathcal E\sim\frac{\delta u_\ell^2}{\tau_{\mathrm{nl}}}\sim\frac{\delta u_\ell^3}{\ell_\perp},\qquad\boxed{\delta u_\ell\sim(\mathcal E\ell_\perp)^{1/3}.}
$$

Define the one-dimensional perpendicular [turbulent energy spectrum](../../../../../../turbulent-energy-spectrum.md) so that $\int E(k_\perp)\,dk_\perp$ measures fluctuation [energy](../../../../../../energy.md) per unit mass. Locality of the spectrum then gives

$$
\delta u_\ell^2\sim\int_{1/\ell_\perp}^{\infty}E(k_\perp)dk_\perp\sim k_\perp E(k_\perp).
$$

Hence

$$
\boxed{E(k_\perp)=C\mathcal E^{2/3}k_\perp^{-5/3},}
$$

where $C$ is a dimensionless normalization constant not determined by the scaling argument. The magnetic and kinetic spectra have the same leading scaling under the assumed Alfvénic amplitude relation.

[Critical balance](../../../../../../critical-balance.md) also determines the scale-dependent anisotropy:

$$
\frac{\ell_\parallel}{v_A}\sim\mathcal E^{-1/3}\ell_\perp^{2/3},\qquad\boxed{k_\parallel\sim\frac{\mathcal E^{1/3}}{v_A}k_\perp^{2/3}.}
$$

Thus the eddies become relatively more elongated along the guide field at smaller perpendicular scales. The $-5/3$ exponent follows under the listed cascade assumptions; it is not established for every imbalanced or aligned [MHD](../../../../../../magnetohydrodynamics.md) state solely by invoking [critical balance](../../../../../../critical-balance.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
