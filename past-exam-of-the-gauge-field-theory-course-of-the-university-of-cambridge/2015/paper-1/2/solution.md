<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A relativistic theory must accommodate the energy-momentum relation $E^2=\mathbf p^2+m^2$, causal interactions and the possibility of particle creation. Promoting the squared relation to a wave equation gives the [Klein-Gordon field](../../../../klein-gordon-field.md) equation

$$
(\partial_t^2-\nabla^2+m^2)\phi=0.
$$

A plane wave $\phi=N e^{-iEt+i\mathbf p\cdot\mathbf x}$ has

$$
\boxed{E=\pm E_{\mathbf p},\qquad E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}.}
$$

The positive and negative branches both solve the local differential equation. Its being second order in time means that specifying only a wavefunction, as in the nonrelativistic Schrödinger equation, is not the complete initial datum.

For a complex scalar, the conserved [Klein-Gordon inner product](../../../../klein-gordon-inner-product.md) comes from the current

$$
j^\mu=i\big(\phi^*\partial^\mu\phi-\phi\partial^\mu\phi^*\big),\qquad
\partial_\mu j^\mu=0.
$$

For the plane wave, **$j^0=2E|N|^2$**, which is negative on the negative-frequency branch. Thus this conserved density cannot be a positive single-particle probability density for arbitrary Klein-Gordon solutions. Merely replacing it by $|\phi|^2$ does not supply the missing conserved relativistic probability law. The [indefinite Klein-Gordon charge density](../../../../indefinite-klein-gordon-charge-density.md) is an obstacle to that naive one-particle interpretation, not evidence that a consistent scalar field theory has negative probabilities.

The [Dirac equation](../../../../dirac-equation.md) is first order,

$$
i\partial_t\psi=H_D\psi,\qquad H_D=\boldsymbol\alpha\cdot\mathbf p+\beta m.
$$

The gamma-matrix anticommutation relations imply $H_D^2=(\mathbf p^2+m^2)I$, so its spectrum again contains $\pm E_{\mathbf p}$. But its conserved [Dirac current](../../../../dirac-current.md) has density $j^0=\psi^\dagger\psi\ge0$. The Dirac equation solves the density-sign difficulty while leaving both energy branches. Treating every negative-energy solution as an ordinary accessible one-electron state would leave the energy unbounded below and permit radiative descent without a stable ground state.

The historical [Dirac sea](../../../../dirac-sea.md) filled the negative-energy electron states and interpreted holes as positive-energy antiparticles. It motivates the [Positron](../../../../positron.md) but is not the general modern explanation: bosons do not obey an exclusion principle and cannot be stabilized by filling a sea. [Quantum field theory](../../../../quantum-field-theory-split.md) instead promotes the fields to operators and interprets negative-frequency modes using antiparticle creation operators.

For a complex scalar field, schematically,

$$
\widehat\phi(x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2E_{\mathbf p}}}
\left(a_{\mathbf p}e^{-ipx}+b_{\mathbf p}^\dagger e^{ipx}\right).
$$

Bosonic commutation relations give a normal-ordered Hamiltonian and conserved charge of the form

$$
:H:=\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}(a^\dagger_{\mathbf p}a_{\mathbf p}+b^\dagger_{\mathbf p}b_{\mathbf p}),
\qquad Q\propto N_a-N_b.
$$

Both particle species have positive excitation energies. The sign-changing scalar current now represents charge, rather than particle probability; opposite charges are physically allowed. The ordinary positive [Fock space](../../../../fock-space.md) norm gives nonnegative probabilities. A real scalar field is its own antiparticle and has no corresponding complex-field U(1) charge.

For the [Dirac field](../../../../dirac-field.md), the analogous expansion contains electron annihilation operators and positron creation operators. Fermionic anticommutation relations turn the negative-frequency contribution into a positive antiparticle excitation energy after the vacuum constant is removed. The [Pauli exclusion principle](../../../../pauli-exclusion-principle.md) and relativistic locality are thereby incorporated in a field description, rather than a postulated infinite population of physical negative-energy electrons. The normal-ordering step removes an additive vacuum constant; it does not by itself settle the separate gravitational vacuum-energy problem.

Interactions can change particle number while conserving total energy, momentum and charge. Trying to localize a particle on its [Compton wavelength](../../../../compton-wavelength.md) scale requires momenta of order its rest mass, where accessible interactions can involve pair creation. A fixed-particle wavefunction is consequently not a general description of such processes. [Creation and annihilation operators](../../../../creation-and-annihilation-operators.md) act between different particle-number sectors, and field interactions describe scattering and production within one framework.

Finally, relativistic causality concerns observables: spacelike separated local bosonic observables commute, while fermionic fields satisfy the appropriate anticommutation conditions. This [microcausality](../../../../microcausality.md) prevents a controllable influence through spacelike separated local operations. Free relativistic one-particle theories remain useful, and low-energy fixed-number approximations can be excellent. What fails is the naive insistence that unrestricted relativistic interactions, positive probabilities, stability and arbitrary particle production all fit an unchanged one-particle Schrödinger picture.[§2.5 complex scalar fields; §5.1–5.3 fermionic quantization and the hole interpretation](../../../../quantum-field-theory-by-david-tong.md)

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
