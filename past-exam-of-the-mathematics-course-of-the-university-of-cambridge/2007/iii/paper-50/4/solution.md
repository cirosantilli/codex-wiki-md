<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**[Antiparticles](../../../../../antiparticle.md) are positive-energy quanta of relativistic [quantum fields](../../../../../quantum-field.md), not physical particles with negative energies.** The negative-frequency part of a [quantum field](../../../../../quantum-field.md) creates these quanta; the distinction between its classical frequency and a state's excitation energy is central to their interpretation.

For a [real scalar field](../../../../../real-scalar-field.md), Hermiticity identifies the two frequency branches:

$$
\phi(x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2E_p}}\left(a_{\mathbf p}e^{-ipx}+a_{\mathbf p}^\dagger e^{ipx}\right).
$$

There is one species of excitation. Its particle is its own [antiparticle](../../../../../antiparticle.md); a single Hermitian scalar cannot carry the nonzero continuous phase charge of a complex field. This does not prevent self-conjugate particles from having other [quantum numbers](../../../../../quantum-number.md).

A [complex scalar field](../../../../../complex-scalar-field.md) is not Hermitian. Its two independent sets of oscillators give

$$
\Phi(x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2E_p}}\left(a_{\mathbf p}e^{-ipx}+b_{\mathbf p}^\dagger e^{ipx}\right),\qquad
\Phi^\dagger(x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2E_p}}\left(a_{\mathbf p}^\dagger e^{ipx}+b_{\mathbf p}e^{-ipx}\right).
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) make $a^\dagger$ and $b^\dagger$ create different positive-energy species. With charge convention fixed by $[Q,\Phi]=-q\Phi$, [normal ordering](../../../../../normal-ordering.md) gives

$$
H=\int\frac{d^3p}{(2\pi)^3}E_p(a_{\mathbf p}^\dagger a_{\mathbf p}+b_{\mathbf p}^\dagger b_{\mathbf p}),\qquad
Q=q\int\frac{d^3p}{(2\pi)^3}(a_{\mathbf p}^\dagger a_{\mathbf p}-b_{\mathbf p}^\dagger b_{\mathbf p}).
$$

Thus $a^\dagger|0\rangle$ and $b^\dagger|0\rangle$ have the same mass and spin but opposite charge. Although $b^\dagger e^{ipx}$ has negative classical frequency, $[H,b^\dagger]=E_pb^\dagger$, so it creates a positive-energy excitation. Two [real scalar fields](../../../../../real-scalar-field.md) can be combined into one complex field; the particle–[antiparticle](../../../../../antiparticle.md) basis diagonalizes the conserved phase charge. Neutrality alone does not require a particle to be self-conjugate.

Locality explains why both branches occur. For the [complex scalar field](../../../../../complex-scalar-field.md),

$$
[\Phi(x),\Phi^\dagger(y)]=\int\frac{d^3p}{(2\pi)^3\,2E_p}\left(e^{-ip\cdot(x-y)}-e^{ip\cdot(x-y)}\right).
$$

At spacelike separation, [Lorentz invariance](../../../../../lorentz-invariance.md) of the [mass shell](../../../../../mass-shell.md) measure permits a frame with equal times; reversing $\mathbf p$ makes the two terms cancel. This is [microcausality](../../../../../microcausality.md). If the [antiparticle](../../../../../antiparticle.md) creation term were omitted, the [commutator](../../../../../commutator.md) would be just a [Wightman function](../../../../../wightman-function.md), generally nonzero at spacelike separation. For example, for a massless scalar at equal times and separation $r>0$, it is $1/(4\pi^2r^2)$. The cancellation is the role of [antiparticle modes and spacelike commutativity](../../../../../antiparticle-modes-and-spacelike-commutativity.md). In a [real scalar field](../../../../../real-scalar-field.md) its self-conjugate creation modes supply the same cancellation.

A [nonrelativistic particle field](../../../../../nonrelativistic-particle-field.md) obeys a first-order time equation and need not contain an antiparticle-creation branch. For example,

$$
\mathcal L=i\Psi^\dagger\partial_t\Psi-\frac{|\nabla\Psi|^2}{2m},\qquad
i\partial_t\Psi=-\frac{\nabla^2}{2m}\Psi,
$$

allows an expansion using only $a_{\mathbf p}e^{-i\mathbf p^2t/(2m)+i\mathbf p\cdot\mathbf x}$ in $\Psi$; its adjoint creates those particles. The basic theory conserves particle number and does not impose a Lorentz-invariant [light cone](../../../../../light-cone.md) locality condition. It often arises from a relativistic [quantum field](../../../../../quantum-field.md) by factoring out the rest-energy oscillation and restricting to a low-energy particle sector, where creation of particle–[antiparticle](../../../../../antiparticle.md) pairs costs roughly $2m$. An [antiparticle](../../../../../antiparticle.md) species can certainly also be treated nonrelativistically with its own field; [antiparticles](../../../../../antiparticle.md) are simply not forced by this nonrelativistic [quantum field](../../../../../quantum-field.md) equation.

Historically, the [Dirac equation](../../../../../dirac-equation.md) has one-particle energy branches $\pm\sqrt{\mathbf p^2+m^2}$. Treating both as ordinary electron energies would leave no lowest-energy one-particle vacuum: an electron could fall through arbitrarily negative levels. The [Dirac sea](../../../../../dirac-sea.md) interpretation fills every negative-energy electron level. The [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md) then blocks further occupation. A missing negative-energy electron is a hole: removing energy $-E$ increases energy by $E$, and removing charge $-e$ leaves charge $+e$. This predicts the positron's mass, spin and opposite electric charge.

The [quantum field theory](../../../../../quantum-field-theory-split.md) account quantizes a [Dirac field](../../../../../dirac-field.md) instead:

$$
\psi(x)=\sum_r\int\frac{d^3p}{(2\pi)^3\sqrt{2E_p}}\left(a_r(\mathbf p)u_r(p)e^{-ipx}+b_r^\dagger(\mathbf p)v_r(p)e^{ipx}\right).
$$

The independent particle and [antiparticle](../../../../../antiparticle.md) operators obey [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md). Before [normal ordering](../../../../../normal-ordering.md), the negative-frequency contribution to the Dirac Hamiltonian has the form $-E_pb_rb_r^\dagger$. Anticommutation rewrites it as $+E_pb_r^\dagger b_r$ plus a vacuum constant. Removing the constant leaves positive particle and [antiparticle](../../../../../antiparticle.md) energies. The charge has opposite signs on the two occupation numbers, and interactions permit pair creation and annihilation while conserving the relevant charges.

There is therefore no need for a literal infinitely populated material sea. The hole picture is a useful fermionic reinterpretation, but it cannot explain bosonic [antiparticles](../../../../../antiparticle.md) through filled-level exclusion, since [bosons](../../../../../boson.md) can multiply occupy a state. [Canonical quantization of a complex scalar field](../../../../../canonical-quantization-of-a-complex-scalar-field.md) supplies them just as consistently. More generally [charge conjugation](../../../../../charge-conjugation.md) relates field representations with opposite internal charges; [real scalar fields](../../../../../real-scalar-field.md) and [Majorana fermions](../../../../../majorana-spinor.md) are self-conjugate exceptions. The relativistic [Fock space](../../../../../fock-space.md) description handles these cases, statistics and changing particle number within one framework.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
