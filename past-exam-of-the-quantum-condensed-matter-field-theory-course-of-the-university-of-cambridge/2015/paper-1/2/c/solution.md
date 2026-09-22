<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider a conventional spin-singlet, weak-coupling, three-dimensional [superconductor](../../../../../superconductor.md). Set $\hbar=k_B=1$ in the microscopic [action](../../../../../action.md) and restore electromagnetic units below. An attraction $\lambda>0$ in an [energy](../../../../../energy-split.md) shell about the [Fermi surface](../../../../../fermi-surface.md) gives a Grassmann [action](../../../../../action.md)

$$
S=\int d\tau\,d^3x\left[\sum_{\sigma=\uparrow,\downarrow}
\bar\psi_\sigma(\partial_\tau+\xi(-i\nabla))\psi_\sigma
-\lambda\bar\psi_\uparrow\bar\psi_\downarrow\psi_\downarrow\psi_\uparrow\right],
\qquad\xi_{\mathbf k}=\epsilon_{\mathbf k}-\mu.
$$

The attractive sign permits pairing even when the single-particle [Fermi gas](../../../../../fermi-gas.md) is otherwise stable. A complex [Hubbard–Stratonovich transformation](../../../../../hubbard-stratonovich-transformation.md) introduces a pair field $\Delta$ proportional at the saddle to $\lambda\langle\psi_\downarrow\psi_\uparrow\rangle$. The [action](../../../../../action.md) is then quadratic in [fermions](../../../../../fermion.md). Integrating them out gives the [BCS pairing-field effective action](../../../../../bcs-pairing-field-effective-action.md)

$$
S_{\rm eff}[\Delta]=\int d\tau\,d^3x\,\frac{|\Delta|^2}{\lambda}
-\operatorname{Tr}\ln\mathcal G^{-1}[\Delta]+\text{constant}.
$$

Here the [trace](../../../../../matrix-trace.md) uses one independent [Nambu spinor](../../../../../nambu-spinor.md) pairing block; a fully doubled particle-hole [representation](../../../../../group-representation.md) instead carries its corresponding one-half factor. At a uniform saddle the [Bogoliubov--de Gennes Hamiltonian](../../../../../bogoliubov-de-gennes-hamiltonian.md) can be written as

$$
\mathcal H_{\rm BdG}(\mathbf k)=\begin{pmatrix}\xi_{\mathbf k}&\Delta\\
\Delta^*&-\xi_{\mathbf k}\end{pmatrix},\qquad
E_{\mathbf k}=\sqrt{\xi_{\mathbf k}^2+|\Delta|^2}.
$$

The negative branch describes the paired vacuum; excitations are [Bogoliubov quasiparticles](../../../../../bogoliubov-quasiparticle.md) mixing particles and holes. Extremizing the [effective action](../../../../../effective-action.md) gives

$$
\boxed{\frac1\lambda=\int_{\rm shell}\frac{d^3k}{(2\pi)^3}
\frac{\tanh(E_{\mathbf k}/2T)}{2E_{\mathbf k}}.}
$$

The physical cutoff or a renormalized interaction is part of the microscopic model; an unregulated contact integral must not be used indiscriminately. With constant [density of states](../../../../../density-of-states.md) $N(0)$ per [spin](../../../../../spin.md) and shell half-width $\Omega_c$, the zero-temperature weak-coupling solution is $\Delta_0\simeq2\Omega_c e^{-1/[N(0)\lambda]}$. The exponentially small scale follows from the logarithmic pairing susceptibility of states near the [Fermi surface](../../../../../fermi-surface.md). For this ideal weak-coupling model, $2\Delta_0/(k_BT_c)\simeq3.53$. The microscopic theory relates the gap, pairing and thermodynamic transition.[pp.1175–1177 and the energy-gap and finite-temperature developments](../../../../../theory-of-superconductivity-by-john-bardeen-and-others.md)

Close to a continuous transition, for fields varying slowly compared with microscopic scales, expand the [effective action](../../../../../effective-action.md) in powers and [gradients](../../../../../gradient.md) of $\Delta$. Its static part is the [Ginzburg-Landau theory of superconductivity](../../../../../ginzburg-landau-theory-of-superconductivity.md):

$$
F=\int d^3x\left[a(T)|\Delta|^2+\frac b2|\Delta|^4+
K\left|\left(-i\nabla-\frac q\hbar\mathbf A\right)\Delta\right|^2
+\frac{|\mathbf B|^2}{2\mu_0}\right],
\qquad q=-2e,\quad b,K>0.
$$

The normalization of $\Delta$ fixes the coefficients; here $a(T)$ changes sign at $T_c$. The uniform minimum has $|\Delta_0|^2=-a/b$ for $a<0$, condensation [free-energy density](../../../../../free-energy-density.md) $-a^2/(2b)$, and characteristic coherence-length scale $\xi=\sqrt{K/|a|}$. Above the transition the minimum is at zero. The quartic stabilization and [gradient](../../../../../gradient.md) cost are precisely the ingredients of [Landau theory](../../../../../landau-theory.md) for a complex [order parameter](../../../../../order-parameter.md). This controlled near-transition expansion supplies a bridge between microscopic [BCS theory](../../../../../bcs-theory.md) and macroscopic magnetic response; its coefficients and validity depend on the material and fluctuation regime.[pp.1364–1367, microscopic expansion near the transition](../../../../../microscopic-derivation-of-the-ginzburg-landau-equations-in-the-theory-of-superconductivity-by-lev-gor-kov.md)

Write $\Delta=(|\Delta_0|+\eta)e^{i\phi}$. The radial fluctuation has positive local restoring curvature, whereas the phase has no local potential in a neutral theory with global $U(1)$ [symmetry](../../../../../symmetry-physics.md). Freezing the amplitude gives

$$
F_\phi=\frac{\rho_s}{2}\int d^3x
\left(\nabla\phi-\frac q\hbar\mathbf A\right)^2,
\qquad\rho_s=2K|\Delta_0|^2.
$$

The neutral case supports a gapless collective phase mode. In the charged case the [electromagnetic field](../../../../../electromagnetic-field.md) couples to this phase rigidity. Under $\mathbf A\mapsto\mathbf A+\nabla\chi$ and $\phi\mapsto\phi+q\chi/\hbar$, the displayed combination is invariant. Locally choosing a gauge with constant phase leaves a quadratic term in $\mathbf A$. Varying the [free energy](../../../../../thermodynamic-free-energy.md) gives the transverse London current and magnetic screening scale,

$$
\mathbf j=-\frac{q^2\rho_s}{\hbar^2}\mathbf A,
\qquad\boxed{\lambda_L^{-2}=\frac{\mu_0q^2\rho_s}{\hbar^2}.}
$$

Combining this relation with static [Maxwell equations](../../../../../maxwell-equations-split.md) gives exponential field penetration, the [Meissner effect](../../../../../meissner-effect.md). Single-valuedness of the pair field around a loop with negligible current gives flux in units $\Phi_0=2\pi\hbar/|q|=\pi\hbar/e$. These are gauge-invariant physical consequences of the condensate stiffness.

For the dynamics, the neutral phase and density mode is reorganized by the Coulomb interaction and the dynamical [electromagnetic field](../../../../../electromagnetic-field.md). In a bulk three-dimensional system the long-wave longitudinal mode has a plasma gap, rather than remaining the neutral sound mode. This is the [Anderson-Higgs mechanism in a superconductor](../../../../../anderson-higgs-mechanism-in-a-superconductor.md): a phase coordinate becomes part of the electromagnetic collective response instead of surviving as an independent massless physical particle. Local [gauge transformations](../../../../../gauge-transformation.md) are redundancies of the description, so a literal breaking of a local redundancy is not an observable. Phase coherence, current response and magnetic screening provide the physical statements.[pp.439–442, plasma oscillations and the charged versus neutral matter spectrum](../../../../../plasmons-gauge-invariance-and-mass-by-philip-warren-anderson.md)

A static Landau functional alone cannot determine that full dynamical spectrum. A two-dimensional film, for example, need not have the same long-wave plasma dispersion as a bulk charged system. Nor does a positive radial curvature automatically guarantee a sharp Higgs amplitude [resonance](../../../../../resonance.md): coupling to quasiparticles and other modes can damp it. The chosen mean-field phase is also a thermodynamic symmetry-breaking description; an isolated finite system can be formulated with definite particle number. **The microscopic pairing saddle, the near-transition Landau expansion and the electromagnetic Anderson-Higgs response describe successive scales of the same superconducting state, with distinct assumptions at each step.**

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
