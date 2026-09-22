<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Condensate depletion](../../../../condensate-depletion.md) means particles outside a macroscopically occupied bosonic single-particle mode. Interactions can deplete that mode even at zero [temperature](../../../../temperature-split.md): the [Bogoliubov transformation](../../../../bogoliubov-transformation.md) mixes creation and [annihilation operators](../../../../annihilation-operator.md), so its [quasiparticle](../../../../quasiparticle.md) vacuum contains particles at nonzero [momentum](../../../../momentum-split.md). A weak homogeneous three-dimensional gas with repulsive scattering length $a_s$ has leading [quantum depletion of a Bose condensate](../../../../quantum-depletion-of-a-bose-condensate.md)

$$
\frac{n-n_0}{n}=\frac8{3\sqrt\pi}\sqrt{na_s^3},\qquad na_s^3\ll1.
$$

Thermal [quasiparticles](../../../../quasiparticle.md) add another contribution. Depletion and normal-fluid density are distinct: a Galilean-invariant fluid can have quantum depletion while retaining its full superfluid [mass](../../../../mass.md) response at zero [temperature](../../../../temperature-split.md).

For the fermionic pairing problem, mean-field decoupling of the [reduced BCS pairing Hamiltonian](../../../../reduced-bcs-pairing-hamiltonian.md) introduces the anomalous amplitude $\Delta$. Each paired Nambu block has diagonal entries $\xi_{\mathbf k},-\xi_{\mathbf k}$ and off-diagonal pairing entries of magnitude $\Delta$. A phase convention with negative off-diagonal entries gives eigenvalues $\pm E_{\mathbf k}$, where $E_{\mathbf k}=\sqrt{\xi_{\mathbf k}^2+\Delta^2}$. Its canonical Bogoliubov rotation yields the [BCS coherence factors](../../../../bcs-coherence-factors.md)

$$
u_{\mathbf k}=\frac1{\sqrt{1+s_{\mathbf k}^2}},\qquad
v_{\mathbf k}=\frac{s_{\mathbf k}}{\sqrt{1+s_{\mathbf k}^2}},\qquad
\frac{v_{\mathbf k}}{u_{\mathbf k}}=\frac{E_{\mathbf k}-\xi_{\mathbf k}}\Delta.
$$

The partner transformation has the complementary sign required by fermionic anticommutation. At zero [temperature](../../../../temperature-split.md) all positive-energy [BCS quasiparticle](../../../../bcs-quasiparticle.md) modes are empty. Expanding the supplied [electron](../../../../electron.md) operator therefore gives

$$
\langle a^\dagger_{\mathbf k\sigma}a_{\mathbf k\sigma}\rangle
=u_{\mathbf k}^2\langle\alpha^\dagger\alpha\rangle
+v_{\mathbf k}^2\langle\alpha\alpha^\dagger\rangle=v_{\mathbf k}^2.
$$

Since $E_{\mathbf k}^2-\xi_{\mathbf k}^2=\Delta^2$,

$$
\boxed{n_{\mathbf k\sigma}=\frac{s_{\mathbf k}^2}{1+s_{\mathbf k}^2}
=\frac12\left(1-\frac{\xi_{\mathbf k}}{\sqrt{\xi_{\mathbf k}^2+\Delta^2}}\right).}
$$

The [electron](../../../../electron.md) occupation is close to one far below the normal-state [Fermi surface](../../../../fermi-surface.md), equals one half at $\xi=0$, and decays toward zero above it. Pairing smooths the Fermi step over an [energy](../../../../energy-split.md) range of order $\Delta$. The positive-energy [quasiparticle](../../../../quasiparticle.md) occupation is instead zero everywhere at this [temperature](../../../../temperature-split.md); the [electron](../../../../electron.md) sea and the [quasiparticle](../../../../quasiparticle.md) vacuum are different descriptions of the same state. At finite [temperature](../../../../temperature-split.md), $n_{\mathbf k\sigma}=[1-(\xi/E)\tanh(E/(2k_BT))]/2$ in the same mean-field model.

<a id="2/image-zero-quasiparticle-occupation-coexists-with-electron-population-above-the-normal-state-fermi-surface"></a>
![](../../../../past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2015/paper-1-electron-quasiparticle-occupation.png)

**[Figure 1](#2/image-zero-quasiparticle-occupation-coexists-with-electron-population-above-the-normal-state-fermi-surface). Zero quasiparticle occupation coexists with electron population above the normal-state Fermi surface**. Original isotropic BCS calculation. The left panel uses an illustrative gap-to-chemical-potential ratio of 0.1; it is not measured mercury or cuprate data.

For a three-dimensional parabolic normal band, the total [density of states](../../../../density-of-states.md) including both spins is $D(\mu)=3N/(2\mu)$. In the weak-gap limit, replace it by this constant across the narrow pairing region and use $\mu\simeq E_F$. The number of [electrons](../../../../electron.md) above the normal-state [Fermi surface](../../../../fermi-surface.md) is

$$
\Delta N\simeq D(\mu)\int_0^\infty\frac12\left(1-\frac\xi{\sqrt{\xi^2+\Delta^2}}\right)d\xi.
$$

The integral is $[\xi-\sqrt{\xi^2+\Delta^2}]_0^\infty/2=\Delta/2$. Therefore the [BCS population above the normal-state Fermi surface](../../../../bcs-population-above-the-normal-state-fermi-surface.md) is

$$
\boxed{\frac{\Delta N}{N}\simeq\frac{3\Delta}{4\mu}.}
$$

The constant-density-of-states approximation and a small gap relative to the [chemical potential](../../../../chemical-potential-split.md) are essential. This is the question's explicitly defined fermionic population measure; it is not the fraction of [electrons](../../../../electron.md) outside a single bosonic condensate orbital.

For an order-of-magnitude mercury estimate, use $T_c\simeq4.2\,\mathrm K$ and the weak-coupling scale $\Delta_0\simeq1.76k_BT_c\simeq0.64\,\mathrm{meV}$, with a representative metallic $\mu\simeq7\,\mathrm{eV}$. These input approximations give **$\Delta N/N\sim7\times10^{-5}$, of order $10^{-4}$**. The use of a weak-coupling gap is an estimate, not an assertion of mercury's exact measured gap.

For a copper oxide, an illustrative gap $20\,\mathrm{meV}$ and effective chemical-potential scale $0.5\,\mathrm{eV}$ give **about three per cent** in this formula. Choosing $0.2$–$1\,\mathrm{eV}$ instead gives roughly $7.5$–$1.5$ per cent. These are explicit example inputs: the paper specifies no compound, doping or band parameters from which a unique number follows. A real cuprate's anisotropic gap, quasi-two-dimensional band and strong correlations require a band-resolved occupation integral, so the reliable contrast is the much larger gap-to-electronic-energy scale, rather than a universal cuprate percentage.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the superconductivity and Quantum Coherence course of the University of Cambridge](../../../split.md)
5. [Superconductivity and Quantum Coherence course of the University of Cambridge](../../../../superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
