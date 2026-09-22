<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A bosonic [coherent state](../../../../coherent-state.md) is an eigenstate of its annihilation operator,

$$
|\alpha\rangle=e^{-|\alpha|^2/2}e^{\alpha a^\dagger}|0\rangle
=e^{-|\alpha|^2/2}\sum_{n=0}^\infty\frac{\alpha^n}{\sqrt{n!}}|n\rangle,
\qquad a|\alpha\rangle=\alpha|\alpha\rangle.
$$

Its mean occupation is $|\alpha|^2$ and its number variance is also $|\alpha|^2$, giving a Poisson number distribution. It has a well-defined complex mean field but fluctuating particle number. Its overlap with another coherent state is $\exp[-(|\alpha|^2+|\beta|^2)/2+\alpha^*\beta]$, so distinct amplitudes need not be orthogonal. For large occupation, a phase-space wave packet has small relative number fluctuations; this does not require an exact self-adjoint phase operator conjugate to a number bounded below.

For a bosonic field, a useful [coherent-field condensate variational state](../../../../coherent-field-condensate-variational-state.md) is

$$
|\psi\rangle=e^{-\bar N/2}\exp\left[\int d^3r\,\psi(\mathbf r)\widehat\Psi^\dagger(\mathbf r)\right]|0\rangle,
\qquad \bar N=\int d^3r\,|\psi|^2.
$$

It obeys $\langle\widehat\Psi(\mathbf r)\rangle=\psi(\mathbf r)$. For a contact-interacting dilute Bose gas, its normal-ordered [energy](../../../../energy-split.md) expectation is

$$
E[\psi]=\int d^3r\left[\frac{\hbar^2}{2m}|\nabla\psi|^2+V|\psi|^2+\frac g2|\psi|^4\right].
$$

Minimizing $E-\mu\bar N$ gives the stationary [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md), $[-\hbar^2\nabla^2/(2m)+V+g|\psi|^2]\psi=\mu\psi$. Its phase gradient determines superfluid flow, while weak-link phase differences give Josephson currents. The complex microscopic expectation supplies the order field used by a mean-field description of a bosonic superfluid.

An exactly fixed-number condensate can instead use the [Hartree product state](../../../../hartree-product-state.md) $(a^\dagger_\varphi)^N|0\rangle/\sqrt{N!}$. Its one-point field expectation vanishes by number conservation, but its one-body [density matrix](../../../../density-matrix-split.md) has a macroscopic eigenvalue. [Off-diagonal long-range order](../../../../off-diagonal-long-range-order.md) expresses that number-conserving criterion. Selecting a phase is a useful thermodynamic symmetry-broken description; it is not a claim that every finite isolated condensate literally has indefinite total number. A plain coherent product also misses interaction-induced quantum depletion, which needs correlations such as those in the Bogoliubov [quasiparticle](../../../../quasiparticle.md) vacuum.

In a spin-singlet superconductor, the corresponding variational state is the [BCS ground state](../../../../bcs-ground-state.md)

$$
|\mathrm{BCS}\rangle=\prod_{\mathbf k}\left(u_{\mathbf k}
+v_{\mathbf k}a^\dagger_{\mathbf k\uparrow}a^\dagger_{-\mathbf k\downarrow}\right)|0\rangle,
\qquad |u_{\mathbf k}|^2+|v_{\mathbf k}|^2=1.
$$

Each block superposes an empty and an occupied pair state. Where $u_{\mathbf k}\ne0$, it can be rewritten as $(\prod u_{\mathbf k})\exp[\sum(v_{\mathbf k}/u_{\mathbf k})a^\dagger_{\mathbf k\uparrow}a^\dagger_{-\mathbf k\downarrow}]|0\rangle$, treating any fully occupied blocks separately. The exponential truncates within each block because a fermionic pair cannot be created twice in the same two modes. This is a [Cooper-pair pseudospin coherent state](../../../../cooper-pair-pseudospin-coherent-state.md), rather than a coherent state of unrestricted ideal [bosons](../../../../boson.md).

The one-electron expectation remains zero in a fermion-parity-even BCS state. Its nonzero microscopic order is the [BCS anomalous average](../../../../bcs-anomalous-average.md) $F_{\mathbf k}=\langle a_{-\mathbf k\downarrow}a_{\mathbf k\uparrow}\rangle=u_{\mathbf k}^*v_{\mathbf k}$. For an attractive interaction written with matrix elements $V_{\mathbf k\mathbf k'}$, the gap is $\Delta_{\mathbf k}=-\sum_{\mathbf k'}V_{\mathbf k\mathbf k'}F_{\mathbf k'}$. Minimization yields the coherence factors and gap equation. [Fermionic coherent states](../../../../fermionic-coherent-state.md) using Grassmann variables are valuable integration tools, but they are not ordinary complex-eigenvalue [electron](../../../../electron.md) states replacing this physical paired [wavefunction](../../../../wave-function-split.md).[1957, variational paired ground state and elementary excitations](../../../../theory-of-superconductivity-by-john-bardeen-and-others.md)

Near the transition, a slowly varying pair field connects the microscopic anomalous average to [Ginzburg-Landau theory of superconductivity](../../../../ginzburg-landau-theory-of-superconductivity.md). The phenomenological complex field has pair charge $-2e$, a phase that controls supercurrent and a magnitude whose normalization is model dependent. It is not the expectation of a single-electron field. [Microscopic derivation of Ginzburg-Landau theory](../../../../microscopic-derivation-of-ginzburg-landau-theory.md) supplies this connection under its stated near-critical assumptions. Pair phase coherence, Josephson [interference](../../../../interference-wave-propagation.md) and flux quantization then become different manifestations of the same macroscopic paired order. Paired-fermion superfluids likewise use a pair order field, while bosonic atomic superfluids can use a one-particle condensate field.

## ↑ Ancestors (13)

1. [3](../3.md)
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
