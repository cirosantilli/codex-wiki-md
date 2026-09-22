# Two-atom neutron diffraction selection

↑ **Parent:** [Neutron diffraction](neutron-diffraction.md)

Choose a one-dimensional [crystal](crystal.md) with cell translation $a$ and two atoms per cell at $0$ and $d=a/2$. Here $d$ is an intracell displacement, distinct from the [interplanar spacing](interplanar-spacing.md) $d_{\mathrm p}$ above. In a single-scattering approximation, a row of $N$ cells has [scattering amplitude](scattering-amplitude.md)

$$
A_N(Q)=\left(b_1+b_2e^{iQd}\right)\sum_{r=0}^{N-1}e^{iQra}.
$$

The sum selects [reciprocal lattice](reciprocal-lattice.md) positions $Q_h=2\pi h/a$ as $N$ becomes large. At these positions, the two-site [crystal basis structure factor](crystal-basis-structure-factor.md) and its squared magnitude are

$$
F_h=b_1+(-1)^h b_2,\qquad
I_h\propto|F_h|^2=
\begin{cases}
(b_1+b_2)^2,&h\text{ even},\\
(b_1-b_2)^2,&h\text{ odd}.
\end{cases}
$$

Consequently $b_1=b_2=b$ gives even reflections of strength $4b^2$ and extinguishes the odd reflections. Choosing $b_1=b$, $b_2=b/2$ instead gives $9b^2/4$ and $b^2/4$: the odd/even ratio is $1/9$. Equal [atomic numbers](atomic-number.md) would not establish equal $b_j$ if the [isotopes](isotope.md) differ. The figure below plots these chosen coefficients, without assigning them to actual elements. Missing reflections can encode destructive [wave interference](interference-wave-propagation.md) within a cell, not the absence of matter at a site.

## ↑ Ancestors (9)

1. [Neutron diffraction](neutron-diffraction.md)
2. [Neutron scattering](neutron-scattering.md)
3. [Neutron](neutron-split.md)
4. [Nucleon](nucleon.md)
5. [Baryon](baryon.md)
6. [Hadron](hadron.md)
7. [Subatomic particle](subatomic-particle.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
