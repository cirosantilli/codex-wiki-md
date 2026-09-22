<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Why [degenerate perturbation theory](../../../degenerate-perturbation-theory.md) is needed.** If several unperturbed states have equal or nearly equal [energy](../../../energy-split.md), a perturbation can mix them at leading order. In that subspace, diagonalize the perturbation matrix rather than using nondegenerate formulas with small [energy](../../../energy-split.md) denominators. The resulting eigenvectors identify the combinations selected by the coupling, and the [eigenvalues](../../../eigenvalue.md) give the leading splitting. Other remote states can then be included perturbatively.

For the [linear combination of atomic orbitals](../../../linear-combination-of-atomic-orbitals.md) description of [molecular hydrogen](../../../molecular-hydrogen.md), equivalent atomic $1s$ states on the two nuclei supply the nearly degenerate starting functions. In an orthonormal two-state model, equal diagonal [energy](../../../energy-split.md) $E_a$ and real hopping $t$ give $E_a\pm t$ and symmetric/antisymmetric combinations. For actual overlapping atomic functions with overlap $S$ and [Hamiltonian](../../../hamiltonian.md) coupling $h$, one instead solves a [generalized eigenvalue problem](../../../generalized-eigenvalue-problem.md):

$$
E_b=\frac{E_a+h}{1+S},\qquad E_{ab}=\frac{E_a-h}{1-S},\qquad \psi_{b,ab}=\frac{\phi_A\pm\phi_B}{\sqrt{2(1\pm S)}}.
$$

The bonding state has enhanced density between the nuclei and the antibonding state a separating node. Two opposite-spin [electrons](../../../electron.md) occupying the [bonding molecular orbital](../../../bonding-orbital.md) describe the simplest closed-shell hydrogen-molecule bond. Electron-electron interaction and nuclear repulsion are needed to calculate a realistic total [binding energy](../../../binding-energy.md); the two-state splitting alone is not the full molecular [energy](../../../energy-split.md).

In the [nearly-free electron model](../../../nearly-free-electron-model.md), the analogous degenerate states are plane waves $|\mathbf k\rangle$ and $|\mathbf k-\mathbf G\rangle$ at a [Bragg scattering](../../../bragg-scattering.md). A [Fourier coefficient](../../../fourier-coefficient.md) $U_{\mathbf G}$ of the [periodic potential](../../../periodic-potential.md) couples them. At exact degeneracy $E_B$, diagonalizing their two-by-two matrix gives

$$
\boxed{E_\pm=E_B+U_0\pm|U_{\mathbf G}|,\qquad E_{\rm gap}=2|U_{\mathbf G}|.}
$$

The associated standing waves place electronic density differently relative to the ionic potential. These are the same gap-opening combinations illustrated in Q1(b). The labels of the two starting [basis](../../../basis.md) states survive as mixed orbital or plane-wave character, rather than independent crossing eigenstates.

**Origin of broad and narrow bands.** Spatially extended s/p-derived orbitals have substantial overlap and therefore large hopping amplitudes and broad bands. More localized d orbitals overlap less strongly and produce narrower bands. A multiorbital tight-binding calculation assigns the on-site orbital energies and hopping matrices, forms Bloch sums, and diagonalizes the resulting matrix at each [wavevector](../../../wavevector.md). Different hopping ranges and orbital [symmetry](../../../symmetry-physics.md) determine the bandwidths and allowed interband coupling. The two-band description retains one broad combination and one nearly flat d-derived combination; a real transition [metal](../../../metal.md) contains several d orbitals and more complicated dispersions.

**Hybridized [eigenvalues](../../../eigenvalue.md) and eigenstates.** Let $|\psi_{\mathbf k}\rangle=a|\phi_{\mathbf k}\rangle+b|\chi_{\mathbf k}\rangle$, in an [orthonormal basis](../../../orthonormal-basis.md). [Hermitian operator](../../../hermitian-operator.md) fixes the reverse coupling to be $V^*$. Projection onto the two components gives

$$
\begin{pmatrix}E_1(\mathbf k)&V\\V^*&E_d\end{pmatrix}\begin{pmatrix}a\\b\end{pmatrix}=E\begin{pmatrix}a\\b\end{pmatrix},\qquad (E_1-E)(E_d-E)-|V|^2=0.
$$

Solving this quadratic yields the [band hybridization](../../../band-hybridization.md) dispersion

$$
\boxed{E_\pm(\mathbf k)=\frac{E_1(\mathbf k)+E_d}{2}\pm\sqrt{\left[\frac{E_1(\mathbf k)-E_d}{2}\right]^2+|V|^2}.}
$$

For nonzero $V$, one [eigenvector](../../../eigenvector.md) representation is $(a,b)\propto(V,E-E_1)$, followed by normalization. Thus the [wavefunctions](../../../wave-function-split.md) exchange broad-band and d-band character through the [avoided crossing](../../../avoided-crossing.md); the levels are equal mixtures at the uncoupled crossing.

At $V=0$, the parabola crosses the horizontal level at $k=\pm k_0$, with $k_0=\sqrt{2mE_d}/\hbar$. For small nonzero $|V|$, the curves avoid crossing with minimum direct separation $2|V|$. The lower branch follows the parabola below the crossing and flattens toward $E_d$ above it; the upper does the opposite. The lower branch satisfies $E_-<E_d$ everywhere and tends to $E_d$ from below as $k\to\infty$, while the upper branch always lies above $E_d$. This is the perfectly flat-band continuum approximation, with zone-boundary intersections excluded as requested.

<a id="4/image-uncoupled-and-weakly-hybridized-broad-flat-bands-with-the-shifted-fermi-radius-and-small-lower-band-slope"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2013-hybridized-bands.png)

**[Figure 7](#4/image-uncoupled-and-weakly-hybridized-broad-flat-bands-with-the-shifted-fermi-radius-and-small-lower-band-slope). Uncoupled and weakly hybridized broad/flat bands, with the shifted Fermi radius and small lower-band slope**.

**Fixed particle number and the larger Fermi sphere.** Denote the uncoupled broad-band Fermi radius by $k_0$ to distinguish it from the new one $K$. With two [spin](../../../spin.md) states, the broad-band [number density](../../../number-density.md) at $V=0$ is $k_0^3/(3\pi^2)$. The stipulated equal population in the flat sector makes the total density twice that value. At zero [temperature](../../../temperature-split.md) and any nonzero hybridization, all occupied states fit into the monotonic lower branch below $E_d$, while the upper branch is empty. Therefore

$$
\frac{K^3}{3\pi^2}=2\frac{k_0^3}{3\pi^2},\qquad \boxed{K=2^{1/3}k_0.}
$$

This is the stated factor increase. It uses fixed total particle number, equal [spin](../../../spin.md) counting, an exactly flat unhybridized band and enough available states below any Brillouin-zone restriction. In generic pairs of dispersive bands both hybridized pockets can remain occupied; then [Fermi-volume conservation in two hybridized electron bands](../../../fermi-volume-conservation-in-two-hybridized-electron-bands.md) fixes a sum of volumes rather than this one radius. The exactly [flat band](../../../flat-band.md) is degenerate at $V=0$, so its initial occupation must be specified, as it is here.

**Fermi-velocity suppression.** Set $\Delta(k)=E_1(k)-E_d$. The exact derivative of the lower branch is

$$
\frac{dE_-}{dk}=\frac{dE_1}{dk}\frac12\left[1-\frac{\Delta(k)}{\sqrt{\Delta(k)^2+4|V|^2}}\right].
$$

At $k=K$, $E_1(K)=2^{2/3}E_d$ and $\Delta(K)=(2^{2/3}-1)E_d>0$. For $|V|\ll\Delta(K)$, the square bracket divided by two is $|V|^2/\Delta(K)^2+O(|V|^4/\Delta(K)^4)$. Since [group velocity](../../../group-velocity.md) is $\hbar^{-1}dE/dk$ and the broad-band reference [velocity](../../../velocity.md) is $v_F^{(1)}=\hbar k_0/m$,

$$
\frac{v_F}{v_F^{(1)}}=\frac{K}{k_0}\frac{|V|^2}{\Delta(K)^2}+O\left(\frac{|V|^4}{E_d^4}\right),
$$

so the [flat-band hybridization Fermi-velocity suppression](../../../flat-band-hybridization-fermi-velocity-suppression.md) is

$$
\boxed{\frac{v_F}{v_F^{(1)}}\simeq\frac{2^{1/3}}{(2^{2/3}-1)^2}\frac{|V|^2}{E_d^2},\qquad A\simeq3.65.}
$$

The reference [velocity](../../../velocity.md) is that of the original broad-band Fermi sphere, not the broad-band slope at the larger $K$; omitting the radius change loses the factor $2^{1/3}$.

The low-temperature qualification becomes more stringent as $V\to0$: the new [chemical potential](../../../chemical-potential-split.md) approaches $E_d$ with $E_d-\mu\simeq |V|^2/\Delta(K)$, and the relevant thermal [energy](../../../energy-split.md) must be small compared with this hybridization scale. At fixed nonzero [temperature](../../../temperature-split.md) the singular flat-band redistribution is not automatically resolved for arbitrarily small coupling. A small but finite narrow-band dispersion can also change the occupation topology.

**[Density of states](../../../density-of-states.md) and magnetism.** For an isotropic three-dimensional branch with [spin](../../../spin.md) degeneracy two,

$$
\frac{g(E_F)}{\mathcal V}=\frac{K^2}{\pi^2|dE_-/dk|_{K}}=\frac{K^2}{\pi^2\hbar v_F}.
$$

A small [Fermi velocity](../../../fermi-velocity.md) therefore produces a large [density of states](../../../density-of-states.md). The localized, partially filled d-derived bands in [iron](../../../iron.md), [cobalt](../../../cobalt.md) and [nickel](../../../nickel.md) place many states close to the [Fermi level](../../../fermi-level.md); broad s/p-derived [conduction bands](../../../conduction-band.md) in [copper](../../../copper.md), [silver](../../../silver.md) and [gold](../../../gold.md) coexist with filled d bands lying below it. This explains the substantially larger Fermi-level [density of states](../../../density-of-states.md) of the former group within the band picture. An exact factor of ten requires the actual band parameters and is not fixed by the two-band toy model.

A high [density of states](../../../density-of-states.md) lowers the kinetic-energy cost of [spin polarization](../../../spin-polarization.md). A repulsive [exchange interaction](../../../exchange-interaction.md) can then satisfy the [Stoner criterion](../../../stoner-criterion.md) and stabilize [ferromagnetism](../../../ferromagnetism.md). With a [single-spin density of states](../../../single-spin-density-of-states.md) $g_s$ and an on-site interaction normalization, the criterion is $Ug_s(E_F)>1$; with spin-summed $g=2g_s$, it is $Ug(E_F)>2$. The large d-state contribution favors this instability in Fe, Co and Ni. The noble [metals](../../../metal.md) do not satisfy the corresponding instability condition in the same ordinary state; this does not imply that they have no weak magnetic response whatsoever.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2013](../../2013-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
