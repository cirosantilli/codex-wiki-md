# Paper 1

↑ **Parent:** [2015](../2015.md)

Original public paper: [Physical PDF pages 746–748](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=746). All three questions are answered. Use $\hbar=c=1$, metric $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$, and canonically normalized gauge-field kinetic terms.

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For an infinitesimal element of the [SO(4) group](../../linear-algebra.md#so-4-group), write $U=I+i\epsilon T+O(\epsilon^2)$. Reality of $U$ makes $T$ purely imaginary; $U^TU=I$ gives $T^T=-T$. Together these imply $T^\dagger=T$, while antisymmetry makes the trace vanish. An antisymmetric four-by-four matrix has $4(4-1)/2=6$ independent entries. Thus six imaginary, Hermitian, antisymmetric, traceless matrices span the [Special orthogonal Lie algebra](../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra) in this convention. The physicists' Hermitian generators differ by a factor of $i$ from the real antisymmetric matrices used for its real Lie algebra.

A nonzero real four-vector has a length and a direction. Proper rotations act transitively on the unit three-sphere, so a gauge choice aligns the scalar [vacuum expectation value](../../quantum-field-theory.md#vacuum-expectation-value) along the fourth coordinate: $\Phi_0=ve_4$. This chooses an orientation of the vacuum without changing its length. Its stabilizer rotates the first three coordinates and is an [SO(3) group](../../linear-algebra.md#so-3-group).

The supplied generators obey

$$
(T^a+T^{a+3})\Phi_0=0,\qquad a=1,2,3.
$$

Hence the three sums are unbroken generators. The orthogonal field combinations

$$
A_\mu^{a,+}=\frac{A_\mu^a+A_\mu^{a+3}}{\sqrt2},\qquad
A_\mu^{a,-}=\frac{A_\mu^a-A_\mu^{a+3}}{\sqrt2}
$$

are respectively the unbroken and broken gauge directions. With $D_\mu=\partial_\mu-igA_\mu^AT^A$, direct action on the vacuum gives

$$
|D_\mu\Phi_0|^2=\frac{g^2v^2}{4}\sum_{a=1}^3(A_\mu^a-A_\mu^{a+3})(A^{a\mu}-A^{a+3,\mu})
=\frac{g^2v^2}{2}\sum_{a=1}^3A_\mu^{a,-}A^{a,-\mu}.
$$

Compare with the vector mass term $m^2A_\mu A^\mu/2$. Therefore

$$
\boxed{m_{a,+}=0,\qquad m_{a,-}=|gv|,\qquad a=1,2,3.}
$$

The [SO(4) vector-Higgs gauge-boson spectrum](../../standard-model.md#so-4-vector-higgs-gauge-boson-spectrum) uses the scalar kinetic normalization printed in the paper, $|D\Phi|^2$. Inserting an additional factor $1/2$ while keeping the same numerical $v$ would instead give $|gv|/\sqrt2$. This is a field-normalization convention, not a disagreement about the broken subgroup. The massless fields generate the residual SO(3) gauge symmetry; they are sums, not three of the six original gauge fields individually.

Multiplying the first three supplied matrices gives

$$
[T^1,T^2]=iT^3,\qquad[T^2,T^3]=iT^1,\qquad[T^3,T^1]=iT^2.
$$

They generate a copy of the [SU(2) Lie algebra](../../semisimple-lie-algebra.md#su-2-lie-algebra). The other triple generates a second copy, and the two commute. Since they span all six dimensions,

$$
\boxed{\mathfrak{so}(4)\cong\mathfrak{su}(2)\oplus\mathfrak{su}(2).}
$$

This is the [two commuting rotation algebras in so4](../../linear-algebra.md#two-commuting-rotation-algebras-in-so4) decomposition. A Lie-algebra isomorphism fixes the local group structure but not its global central identifications. The [Spin(4) double cover](../../semisimple-lie-algebra.md#spin-4-double-cover) gives

$$
\boxed{SO(4)\cong\big(SU(2)\times SU(2)\big)/\{(I,I),(-I,-I)\}.}
$$

Thus SO(4) is not globally the direct product of the two simply connected groups. The unbroken diagonal Lie algebra integrates to SO(3), with the same simultaneous central sign already identified. This distinguishes the gauge algebra, its covering group and the actual group acting faithfully on the four-vector.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A relativistic theory must accommodate the energy-momentum relation $E^2=\mathbf p^2+m^2$, causal interactions and the possibility of particle creation. Promoting the squared relation to a wave equation gives the [Klein-Gordon field](../../quantum-field-theory.md#klein-gordon-field) equation

$$
(\partial_t^2-\nabla^2+m^2)\phi=0.
$$

A plane wave $\phi=N e^{-iEt+i\mathbf p\cdot\mathbf x}$ has

$$
\boxed{E=\pm E_{\mathbf p},\qquad E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}.}
$$

The positive and negative branches both solve the local differential equation. Its being second order in time means that specifying only a wavefunction, as in the nonrelativistic Schrödinger equation, is not the complete initial datum.

For a complex scalar, the conserved [Klein-Gordon inner product](../../quantum-field-theory.md#klein-gordon-inner-product) comes from the current

$$
j^\mu=i\big(\phi^*\partial^\mu\phi-\phi\partial^\mu\phi^*\big),\qquad
\partial_\mu j^\mu=0.
$$

For the plane wave, **$j^0=2E|N|^2$**, which is negative on the negative-frequency branch. Thus this conserved density cannot be a positive single-particle probability density for arbitrary Klein-Gordon solutions. Merely replacing it by $|\phi|^2$ does not supply the missing conserved relativistic probability law. The [indefinite Klein-Gordon charge density](../../quantum-field-theory.md#indefinite-klein-gordon-charge-density) is an obstacle to that naive one-particle interpretation, not evidence that a consistent scalar field theory has negative probabilities.

The [Dirac equation](../../relativistic-quantum-field.md#dirac-equation) is first order,

$$
i\partial_t\psi=H_D\psi,\qquad H_D=\boldsymbol\alpha\cdot\mathbf p+\beta m.
$$

The gamma-matrix anticommutation relations imply $H_D^2=(\mathbf p^2+m^2)I$, so its spectrum again contains $\pm E_{\mathbf p}$. But its conserved [Dirac current](../../classical-field-theory.md#dirac-current) has density $j^0=\psi^\dagger\psi\ge0$. The Dirac equation solves the density-sign difficulty while leaving both energy branches. Treating every negative-energy solution as an ordinary accessible one-electron state would leave the energy unbounded below and permit radiative descent without a stable ground state.

The historical [Dirac sea](../../relativistic-quantum-field.md#dirac-sea) filled the negative-energy electron states and interpreted holes as positive-energy antiparticles. It motivates the [Positron](../../physics.md#positron) but is not the general modern explanation: bosons do not obey an exclusion principle and cannot be stabilized by filling a sea. [Quantum field theory](../../quantum-field-theory.md) instead promotes the fields to operators and interprets negative-frequency modes using antiparticle creation operators.

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

Both particle species have positive excitation energies. The sign-changing scalar current now represents charge, rather than particle probability; opposite charges are physically allowed. The ordinary positive [Fock space](../../quantum-field-theory.md#fock-space) norm gives nonnegative probabilities. A real scalar field is its own antiparticle and has no corresponding complex-field U(1) charge.

For the [Dirac field](../../relativistic-quantum-field.md#dirac-field), the analogous expansion contains electron annihilation operators and positron creation operators. Fermionic anticommutation relations turn the negative-frequency contribution into a positive antiparticle excitation energy after the vacuum constant is removed. The [Pauli exclusion principle](../../tensor-product-of-quantum-systems.md#pauli-exclusion-principle) and relativistic locality are thereby incorporated in a field description, rather than a postulated infinite population of physical negative-energy electrons. The normal-ordering step removes an additive vacuum constant; it does not by itself settle the separate gravitational vacuum-energy problem.

Interactions can change particle number while conserving total energy, momentum and charge. Trying to localize a particle on its [Compton wavelength](../../mathematical-physics.md#compton-wavelength) scale requires momenta of order its rest mass, where accessible interactions can involve pair creation. A fixed-particle wavefunction is consequently not a general description of such processes. [Creation and annihilation operators](../../quantum-harmonic-oscillator.md#creation-and-annihilation-operators) act between different particle-number sectors, and field interactions describe scattering and production within one framework.

Finally, relativistic causality concerns observables: spacelike separated local bosonic observables commute, while fermionic fields satisfy the appropriate anticommutation conditions. This [microcausality](../../relativistic-quantum-field.md#microcausality) prevents a controllable influence through spacelike separated local operations. Free relativistic one-particle theories remain useful, and low-energy fixed-number approximations can be excellent. What fails is the naive insistence that unrestricted relativistic interactions, positive probabilities, stability and arbitrary particle production all fit an unchanged one-particle Schrödinger picture.[§2.5 complex scalar fields; §5.1–5.3 fermionic quantization and the hole interpretation](../../physics-bibliography.md#quantum-field-theory-by-david-tong)

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

At leading order in [quantum electrodynamics](../../perturbative-quantum-field-theory.md#quantum-electrodynamics), the electron-positron pair annihilates into one virtual [photon](../../quantum-mechanics.md#photon), which produces the muon-antimuon pair. This is an s-channel [Feynman diagram](../../perturbative-quantum-field-theory.md#feynman-diagram) with $q=p_-+p_+=k_-+k_+$ and $q^2=s$. No QED vertex changes an electron directly into a muon, so there is no corresponding single-photon t-channel flavor-changing diagram.

<a id="3/image-leading-order-electron-positron-annihilation-into-a-muon-pair-through-a-virtual-photon"></a>
![](../../past-exam-of-the-gauge-field-theory-course-of-the-university-of-cambridge/2015/paper-1-muon-pair-diagram.png)

**[Figure 1](#3/image-leading-order-electron-positron-annihilation-into-a-muon-pair-through-a-virtual-photon). Leading-order electron-positron annihilation into a muon pair through a virtual photon**. Original s-channel diagram. Arrows follow fermion-number flow; each labelled external four-momentum refers to the physical incoming or outgoing particle, and the virtual photon carries q from left to right.

Each charged-fermion vertex contributes $-ie\gamma^\mu$, the internal photon contributes $-ig_{\mu\nu}/(q^2+i0)$ in Feynman gauge, and external legs supply incoming $u(p_-),\bar v(p_+)$ and outgoing $\bar u(k_-),v(k_+)$. Their ordered contraction gives the stated amplitude. The overall convention-dependent phase does not affect its squared modulus.

For unpolarized scattering, average over the two spin choices of each incoming particle and sum over outgoing spins. The identities $\sum u\bar u=\not{p}+m$ and $\sum v\bar v=\not{p}-m$, together with $\gamma^0(\gamma^\mu)^\dagger\gamma^0=\gamma^\mu$, convert the products into [fermion spin sums](../../relativistic-quantum-field.md#fermion-spin-sum):

$$
\boxed{\overline{|\mathcal M|^2}=\frac{e^4}{4s^2}
\operatorname{tr}\big[(\not{p}_+-m_e)\gamma_\mu(\not{p}_-+m_e)\gamma_\nu\big]
\operatorname{tr}\big[(\not{k}_-+m_\mu)\gamma^\mu(\not{k}_+-m_\mu)\gamma^\nu\big].}
$$

The factor $1/4$ averages the initial spins; there is no additional average over the final ones. In the massless limit the first trace is $4(p_{+\mu}p_{-\nu}+p_{+\nu}p_{-\mu}-g_{\mu\nu}p_+\cdot p_-)$, with the analogous expression for the outgoing current. Contracting gives

$$
\overline{|\mathcal M|^2}=\frac{8e^4}{s^2}
\left[(p_+\cdot k_-)(p_-\cdot k_+)+(p_+\cdot k_+)(p_-\cdot k_-)\right].
$$

In the [centre-of-mass frame](../../special-relativity.md#center-of-momentum-frame), every external energy is $E_{\rm cm}/2$. Choose $p_-$ along $+z$ and let $k_-$ make angle $\theta$ with it. The dot products are $p_-\cdot k_-=p_+\cdot k_+=s(1-\cos\theta)/4$ and $p_-\cdot k_+=p_+\cdot k_-=s(1+\cos\theta)/4$. Hence

$$
\boxed{\overline{|\mathcal M|^2}=e^4(1+\cos^2\theta).}
$$

The [electron-positron annihilation into a muon pair](../../perturbative-quantum-field-theory.md#electron-positron-annihilation-into-a-muon-pair) cross-section is therefore

$$
\frac{d\sigma}{d\Omega}=\frac{\alpha^2}{4s}(1+\cos^2\theta).
$$

Using $d\Omega=2\pi\,d(\cos\theta)$ gives

$$
\boxed{\sigma=\frac{4\pi\alpha^2}{3s}=\frac{4\pi\alpha^2}{3E_{\rm cm}^2}.}
$$

In ordinary units this becomes $4\pi\alpha^2(\hbar c)^2/(3E_{\rm cm}^2)$. It is the leading high-energy QED result: finite masses, radiative corrections and weak-interaction exchange modify the prediction outside that approximation.

Cross-section measurements can test spin assignments when the interaction and charges are specified. For example, keeping spin-half electrons but replacing the final muons by minimally coupled charged spin-zero particles replaces the fermion current by a momentum-difference current. In the massless limit, [scalar-pair production by fermion annihilation](../../relativistic-quantum-field.md#scalar-pair-production-by-fermion-annihilation) gives $d\sigma/d\Omega=\alpha^2\sin^2\theta/(8s)$ and total $\pi\alpha^2/(3s)$. Its central angular peak differs from the fermionic $1+\cos^2\theta$ distribution.

Thus angular distributions, polarization information and suitably modeled rates distinguish spin hypotheses. A single total rate without assumptions about the couplings or the initial species does not independently establish both spins; changing interactions can mimic normalizations. The predicted fermion result is a testable consequence of the spin-half QED model, rather than a model-independent inference of spin from any one observed cross-section.

## ↑ Ancestors (11)

1. [2015](../2015.md)
2. [Past exam of the gauge field theory course of the University of Cambridge](../../past-exam-of-the-gauge-field-theory-course-of-the-university-of-cambridge.md)
3. [Gauge Field Theory course of the University of Cambridge](../../university-of-cambridge.md#gauge-field-theory-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
