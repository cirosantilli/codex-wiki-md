<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The absorptive [dielectric function](../../../../dielectric-function.md) counts optically accessible [electron-hole pairs](../../../../electron-hole-pair.md). In the electric dipole approximation the perturbation is proportional to $\mathbf a\cdot\hat{\mathbf p}$, with $\mathbf a$ the [light](../../../../light.md) [polarization](../../../../polarization-waves.md) and $\hat{\mathbf p}$ the electronic [momentum operator](../../../../momentum-operator.md). The squared [matrix element](../../../../matrix-element.md) between occupied valence and empty conduction states is the transition strength; it includes [polarization](../../../../polarization-waves.md) and band-symmetry selection rules. The sums enumerate initial and final subbands. [photon](../../../../photon.md) [momentum](../../../../momentum-split.md) is negligible on the crystal-momentum scale, so the transition is approximately vertical in the in-plane wavevector $\mathbf k$.

For each subband pair, $C$ is the constant-transition-energy contour in the two-dimensional [Brillouin zone](../../../../brillouin-zone.md). Its line element is $dl$, and the reciprocal gradient weights the states satisfying [energy](../../../../energy-split.md) conservation. Specifically, the [level-set representation of the joint density of states](../../../../level-set-representation-of-the-joint-density-of-states.md) is

$$
\int d^2k\,\delta\!\left(E_{n'}(\mathbf k)-E_n(\mathbf k)-\hbar\omega\right)=\int_C\frac{dl}{|\nabla_{\mathbf k}(E_{n'}-E_n)|}.
$$

A small [energy](../../../../energy-split.md) gradient means many nearly resonant states; a vanishing gradient can produce a [Van Hove singularity](../../../../van-hove-singularity.md) or an edge. The displayed expression suppresses overall optical prefactors and assumes the [momentum](../../../../momentum-split.md) [matrix element](../../../../matrix-element.md) is approximately constant along each contour. More generally it stays inside that integral. Occupation factors $f_v-f_c$ are also implicit; at low [temperature](../../../../temperature-split.md) in an undoped well the relevant valence states are full and the conduction states empty. This is the independent-particle continuum contribution from [Fermi's golden rule](../../../../fermi-s-golden-rule.md). Bound [excitons](../../../../exciton.md) add optical resonances below the corresponding free-pair thresholds.

The [GaAs four-band model](../../../../gaas-four-band-model.md) is rooted in bonding and [spin-orbit coupling](../../../../spin-orbit-interaction.md). Near the zone centre, the conduction edge is predominantly s-like and antibonding, while the upper valence manifold is predominantly p-like. Combining [orbital angular momentum](../../../../orbital-angular-momentum.md) $l=1$ with [spin](../../../../spin.md) $s=1/2$ splits the six p-derived states into a $j=3/2$ quartet and a lower $j=1/2$ doublet. The latter is the [split-off valence band](../../../../split-off-valence-band.md). Within the upper quartet, the $m_j=\pm3/2$ and $m_j=\pm1/2$ branches, defined relative to a propagation or quantization direction, have different curvatures and are called [heavy holes](../../../../heavy-hole.md) and [light holes](../../../../light-hole.md). They coincide at the unstrained bulk zone centre but need not remain degenerate in a well. The conduction edge is a [spin](../../../../spin.md) doublet. Thus “four bands” counts conduction, heavy-hole, light-hole and split-off branches, including their [spin](../../../../spin.md) multiplicities; it does not count four individual states. Positive hole masses describe the downward valence curvature, whereas the conduction curvature is upward.

For the final [exciton](../../../../exciton.md) comparison, define the [reduced mass](../../../../reduced-mass.md) $\mu_j$ and screened [exciton](../../../../exciton.md) Rydberg $R_j^*$ by

$$
\frac1{\mu_j}=\frac1{m_e^*}+\frac1{m_{h,j}^*},\qquad R_j^*=\frac{\mu_j}{m_e}\frac{13.6\,\mathrm{eV}}{12.8^2}.
$$

The resulting $(\mu_j/m_e,R_j^*)$ are approximately $(0.05948,4.937\,\mathrm{meV})$ for [heavy holes](../../../../heavy-hole.md), $(0.03646,3.027\,\mathrm{meV})$ for [light holes](../../../../light-hole.md) and $(0.04631,3.844\,\mathrm{meV})$ for split-off holes. In the ideal [two-dimensional exciton](../../../../two-dimensional-exciton.md) model, the first two optically active internal states lie $4R_j^*$ and $4R_j^*/9$ below their continuum edge. Their separation is $32R_j^*/9$, independent of a common threshold offset. The corresponding three-dimensional separation would be only $3R_j^*/4$. The listed peak spacings specified for this theoretical spectrum give

$$
\begin{array}{c|c|c|c}
\text{subband family}&\text{listed successive pair spacings / meV}&\text{2D prediction / meV}&\text{3D prediction / meV}\\\hline
\mathrm{hh},\ n=1,2,3&18,\ 18,\ 17&17.56&3.70\\
\mathrm{lh},\ n=1,2,3&11,\ 11,\ 10&10.76&2.27
\end{array}
$$

Here each pair comprises the stronger lower-energy peak and its weaker nearby companion, in the order associated with the continuum edges calculated in part (c). **The approximately 18-meV and 11-meV pair splittings support the two-dimensional series and are incompatible with the three-dimensional series at the supplied masses and permittivity.** Equivalently, for a two-dimensional pair with energies $E_1,E_2$, the inferred edge is $E_2+(E_2-E_1)/8$; the observed pair splittings predict ground-state bindings around 20 and 12 meV, close to $4R_j^*$.

Absolute agreement should not be overstated. For example, the stated square-well parameters give the first heavy-hole edge $1.56390$ eV and the first light-hole edge $1.59161$ eV. Their ideal two-dimensional peak predictions are approximately $(1.54415,1.56170)$ eV and $(1.57950,1.59027)$ eV, respectively. The listed peaks are lower by about 1–2 meV across the families; rounded parameters and this simple effective-mass model do not reproduce every absolute [energy](../../../../energy-split.md) exactly. No gap, width or mass has been silently adjusted to fit them. The peak-spacing comparison remains useful because it avoids a common edge offset. The split-off transitions predicted by the four-band data are discussed separately in part (c), rather than assigned fictitious extra peaks.

At 300 K, $k_BT\simeq25.9$ meV, whereas the ideal ground-state binding energies are only about $19.7$, $12.1$ and $15.4$ meV; excited states are still more weakly bound. **None of these series is expected to remain a clearly resolved, robust bound-exciton peak at room [temperature](../../../../temperature-split.md) in this simple estimate.** Thermal ionization and [phonon](../../../../phonon.md) broadening work against their visibility. This is a scale argument, not a theorem that the [exciton](../../../../exciton.md) population or all Coulomb-enhanced absorption becomes exactly zero: actual observability also requires temperature-dependent gaps, linewidths, screening and carrier density, which are not supplied.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
