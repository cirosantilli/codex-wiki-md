<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Start from [electrons](../../../../electron.md) moving in the periodic equilibrium ionic potential. Displace ion $l$ by $\mathbf u_l$ and expand its contribution as $V(\mathbf r-\mathbf R_l-\mathbf u_l)\simeq V(\mathbf r-\mathbf R_l)-\mathbf u_l\cdot\nabla V(\mathbf r-\mathbf R_l)$. Quantizing the harmonic [normal modes](../../../../normal-mode.md) expresses $\mathbf u_l$ as a sum of creation and [annihilation operators](../../../../annihilation-operator.md) with displacement scale $\sqrt{\hbar/(2\rho_{\rm ion}V\omega_{\mathbf q})}$ for a single simple branch. Expanding the electronic field in [bloch states](../../../../bloch-state.md) then gives a band-projected [Fröhlich Hamiltonian](../../../../frohlich-hamiltonian.md)

$$
H=H_0+V_{e\text{-}ph},\qquad H_0=\sum_{\mathbf k\sigma}\epsilon_{\mathbf k}c_{\mathbf k\sigma}^{\dagger}c_{\mathbf k\sigma}+\sum_{\mathbf q}\Omega_{\mathbf q}b_{\mathbf q}^{\dagger}b_{\mathbf q},
$$



$$
V_{e\text{-}ph}=\sum_{\mathbf k\mathbf q\sigma}M_{\mathbf q}c_{\mathbf k+\mathbf q,\sigma}^{\dagger}c_{\mathbf k\sigma}(b_{\mathbf q}+b_{-\mathbf q}^{\dagger}),\qquad \Omega_{\mathbf q}=\hbar\omega_{\mathbf q}.
$$

Here $c,c^{\dagger}$ obey [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) and remove/create an [electron](../../../../electron.md) with [crystal momentum](../../../../crystal-momentum.md) $\mathbf k$ and [spin](../../../../spin.md) $\sigma$; $b,b^{\dagger}$ are [boson](../../../../boson.md) operators for lattice modes. The [matrix element](../../../../matrix-element.md) $M_{\mathbf q}$ contains the derivative of the ionic potential, [phonon polarization](../../../../phonon-polarization.md), displacement normalization and electronic [wavefunction](../../../../wave-function-split.md) overlaps. With phases chosen appropriately, $M_{-\mathbf q}=M_{\mathbf q}^*$ ensures a [Hermitian](../../../../hermitian-operator.md) Hamiltonian. The displayed one-band, one-branch notation suppresses additional branch and band labels. “[Fröhlich Hamiltonian](../../../../frohlich-hamiltonian.md)” here means the linear electron-phonon model used in the question; it is not a requirement to use specifically the polar-optical-phonon coupling of a polar [semiconductor](../../../../semiconductor-split.md). A harmonic lattice, small displacements and a weak enough coupling to organize [perturbation theory](../../../../perturbation-theory.md) are the underlying approximations.

The [Fröhlich canonical transformation](../../../../frohlich-canonical-transformation.md) removes real linear [phonon](../../../../phonon.md) operators from the electron-only effective problem to first order. Choose an [anti-Hermitian](../../../../skew-hermitian-matrix.md) $S$ with $[S,H_0]=-V_{e\text{-}ph}$. For $A_{\mathbf k\mathbf q\sigma}=c_{\mathbf k+\mathbf q,\sigma}^{\dagger}c_{\mathbf k\sigma}$ and $\Delta_{\mathbf k\mathbf q}=\epsilon_{\mathbf k+\mathbf q}-\epsilon_{\mathbf k}$, one possible generator is

$$
S=\sum_{\mathbf k\mathbf q\sigma}M_{\mathbf q}A_{\mathbf k\mathbf q\sigma}\left(\frac{b_{\mathbf q}}{\Delta_{\mathbf k\mathbf q}-\Omega_{\mathbf q}}+\frac{b_{-\mathbf q}^{\dagger}}{\Delta_{\mathbf k\mathbf q}+\Omega_{\mathbf q}}\right).
$$

Its [Hermitian](../../../../hermitian-operator.md) conjugate is its negative after relabelling momenta. The [Baker--Campbell--Hausdorff formula](../../../../baker-campbell-hausdorff-formula.md) gives

$$
e^SHe^{-S}=H_0+\frac12[S,V_{e\text{-}ph}]+O(M^3).
$$

The [commutator](../../../../commutator.md) describes virtual emission and absorption of a [phonon](../../../../phonon.md). [normal ordering](../../../../normal-ordering.md) yields an electron-electron term as well as one-electron [energy](../../../../energy-split.md) renormalizations and [phonon](../../../../phonon.md) terms. Retain the former, absorb single-particle shifts into $\epsilon_{\mathbf k}$ and eliminate the explicit [phonon](../../../../phonon.md) sector. For elastic pair scattering the two virtual time orderings have the combined amplitude

$$
V_{\rm eff}(\mathbf q,\Delta)=|M_{\mathbf q}|^2\left(\frac1{\Delta-\Omega_{\mathbf q}}-\frac1{\Delta+\Omega_{\mathbf q}}\right)=\frac{2|M_{\mathbf q}|^2\Omega_{\mathbf q}}{\Delta^2-\Omega_{\mathbf q}^2}.
$$

Using the usual factor one-half to count unordered pairs gives the coefficient in the printed Hamiltonian, with $\Delta=\epsilon_{\mathbf k}-\epsilon_{\mathbf k-\mathbf q}$. The two outgoing momenta are $\mathbf k-\mathbf q$ and $\mathbf k'+\mathbf q$, so total [momentum](../../../../momentum-split.md) and the [spins](../../../../spin.md) are conserved. A fully off-shell effective operator can instead use symmetrized denominators for both external legs; the displayed expression is the usual elastic-scattering reduction. Eliminating nearly resonant real [phonons](../../../../phonon.md) requires more care than this second-order construction.

For $|\Delta|<\Omega_{\mathbf q}$ the denominator is negative: **virtual [phonon](../../../../phonon.md) exchange is attractive in this low-energy channel**. Physically, an [electron](../../../../electron.md) changes the ionic density and a second [electron](../../../../electron.md) can gain [energy](../../../../energy-split.md) by responding to the delayed distortion. This is a retarded interaction, not an unscreened instantaneous attraction at every [energy](../../../../energy-split.md) transfer. At large transfer the sign changes, and screened Coulomb repulsion must also be included when deciding the net low-energy pairing strength. The connection between lattice dynamics and [superconductivity](../../../../superconductivity-split.md) is supported by the isotope effect, but the mathematical attraction alone does not determine a measured transition [temperature](../../../../temperature-split.md).[pp. 55–57, lattice-coupling mechanism and isotope-effect motivation](../../../../electron-phonon-interactions-and-superconductivity-by-john-bardeen.md)

For the pair calculation, make the model restrictions explicit. The filled [Fermi sea](../../../../fermi-sea.md) is inert, and $|0\rangle$ denotes that sea with no added particles, not an empty electronic vacuum. Project the interaction onto the previously empty shell $0\le\xi_{\mathbf k}\le D$, where $\xi_{\mathbf k}=\hbar^2k^2/(2m)-E_F$ and $D=\hbar\omega_D$. Measure the added-pair [energy](../../../../energy-split.md) relative to $2E_F$; this is the negative $E$ in the final formula. If absolute one-electron energies are retained in the preceding [eigenvalue](../../../../eigenvalue.md) equation, its [eigenvalue](../../../../eigenvalue.md) must instead be $E_{\rm abs}=2E_F+E$. A shell-restricted state would not in general be an exact eigenstate of the completely unprojected, all-momentum contact Hamiltonian.

Write $g=\gamma^2>0$ and $|\mathbf k\rangle=c_{-\mathbf k\downarrow}^{\dagger}c_{\mathbf k\uparrow}^{\dagger}|0\rangle$. Within the zero-total-momentum pair subspace the two opposite-spin terms cancel the interaction's factor one-half, while same-spin s-wave terms cancel by fermionic antisymmetry. Thus the projected Hamiltonian acts as

$$
H'_{\rm pair}|\mathbf k\rangle=2\xi_{\mathbf k}|\mathbf k\rangle-g\sum_{\langle\mathbf p\rangle}|\mathbf p\rangle.
$$

For $|\Psi\rangle=\sum_{\langle\mathbf k\rangle}\varphi_{\mathbf k}|\mathbf k\rangle$ and $C=\sum_{\langle\mathbf k\rangle}\varphi_{\mathbf k}$, matching each basis coefficient gives

$$
(E-2\xi_{\mathbf k})\varphi_{\mathbf k}=-gC,\qquad \boxed{\varphi_{\mathbf k}=-\frac{\gamma^2C}{E-2\xi_{\mathbf k}}.}
$$

This is the stated coefficient formula in the consistent Fermi-level [energy](../../../../energy-split.md) convention. Its even dependence on $\mathbf k$ produces an even orbital state with a [spin](../../../../spin.md) singlet. The constant $C$ is fixed up to an overall phase by normalization; for a [bound state](../../../../bound-state.md), $|C|^{-2}=g^2\sum_{\langle\mathbf k\rangle}(E-2\xi_{\mathbf k})^{-2}$. It cannot be set to zero for the nontrivial bound solution.

Put $E=-B$ with $B>0$ and impose the sum defining $C$:

$$
1=g\sum_{\langle\mathbf k\rangle}\frac1{2\xi_{\mathbf k}+B}\simeq g\rho(E_F)\int_0^D\frac{d\xi}{2\xi+B}=\frac{g\rho(E_F)}2\log\frac{2D+B}{B}.
$$

Here $\rho(E_F)$ counts orbital states for one [spin](../../../../spin.md) species, as appropriate to the unrestricted $\mathbf k$ sum in this pair basis, and is approximately constant over the thin shell. If a two-spin total [density of states](../../../../density-of-states.md) is used, it must be divided by two in this integral. State-counting and the volume convention in $g$ and $\rho$ must be consistent. With $\xi=g\rho(E_F)$ as the paper's dimensionless coupling, inversion yields

$$
\boxed{E=-\frac{2\hbar\omega_D}{e^{2/\xi}-1}\simeq-2\hbar\omega_D e^{-2/\xi}\quad(\xi\ll1).}
$$

The first approximation is the constant-density-of-states, restricted-shell model; the final exponential additionally assumes weak attraction. The binding [energy](../../../../energy-split.md) is nonanalytic at zero coupling, so a finite-order power expansion in $g$ cannot produce it.

Cooper's problem asks whether two [electrons](../../../../electron.md) added above an inert [Fermi sea](../../../../fermi-sea.md) bind despite Pauli exclusion of lower states. **An arbitrarily weak net attraction binds a zero-momentum singlet below the free-pair threshold**, because the near-Fermi-surface integral diverges logarithmically as $B\downarrow0$. Its [wavefunction](../../../../wave-function-split.md) draws on many time-reversed [momentum](../../../../momentum-split.md) states and becomes dominated by a narrow region near the [Fermi surface](../../../../fermi-surface.md) at weak coupling; the corresponding pair is spatially extended. This establishes a [Cooper instability](../../../../cooper-instability.md) of the unpaired reference state.[pp. 1189–1190, two added particles above the filled sea and the bound-state criterion](../../../../bound-electron-pairs-in-a-degenerate-fermi-gas-by-leon-neil-cooper.md) The full superconducting [ground state](../../../../ground-state.md) needs a coherent many-electron treatment in which overlapping pairs and the reorganized sea are included. [BCS theory](../../../../bcs-theory.md) supplies that step; the two-electron binding scale alone is neither a calculation of the many-body gap nor a derivation of zero resistance.[pp. 1175–1177, paired many-electron ground state and excitation gap](../../../../theory-of-superconductivity-by-john-bardeen-and-others.md)

## ↑ Ancestors (13)

1. [2](../2.md)
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
