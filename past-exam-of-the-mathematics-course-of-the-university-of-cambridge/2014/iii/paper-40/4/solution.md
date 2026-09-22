<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [real scalar field](../../../../../real-scalar-field.md), the mostly-plus [Minkowski metric](../../../../../minkowski-metric.md) gives a positive kinetic energy. Its [canonical momentum](../../../../../canonical-momentum.md) and [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) are

$$
\pi=\frac{\partial\mathcal L}{\partial\dot\phi}=\dot\phi,
\qquad
H=\frac12\int d^3\boldsymbol x\,
\left[\pi^2+(\boldsymbol\nabla\phi)^2+m^2\phi^2\right].
$$

The [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is $(\Box-m^2)\phi=0$, or $(\partial_t^2-\nabla^2+m^2)\phi=0$. [Canonical quantization of a real scalar field](../../../../../canonical-quantization-of-a-real-scalar-field.md) promotes the fields to Hermitian operators and replaces the equal-time [Poisson brackets](../../../../../poisson-bracket.md) by [canonical commutation relations](../../../../../canonical-commutation-relation.md):

$$
[\phi(t,\boldsymbol x),\pi(t,\boldsymbol y)]=i\delta^{(3)}(\boldsymbol x-\boldsymbol y),
\qquad [\phi(t,\boldsymbol x),\phi(t,\boldsymbol y)]=[\pi(t,\boldsymbol x),\pi(t,\boldsymbol y)]=0.
$$

The [Heisenberg equation of motion](../../../../../heisenberg-equation-of-motion.md) then gives $\dot\phi=\pi$ and $\dot\pi=\nabla^2\phi-m^2\phi$, so the classical field equation remains an operator identity. Products at coincident points need a regulator; equivalently, the field is an [operator-valued distribution](../../../../../operator-valued-distribution.md).

Resolve the free field into positive- and negative-frequency [plane waves](../../../../../plane-wave.md). With $E_{\boldsymbol k}=\sqrt{|\boldsymbol k|^2+m^2}$ and $k\cdot x=-E_{\boldsymbol k}t+\boldsymbol k\cdot\boldsymbol x$,

$$
\phi(x)=\int\frac{d^3\boldsymbol k}{(2\pi)^3\sqrt{2E_{\boldsymbol k}}}
\left[a(\boldsymbol k)e^{ik\cdot x}+a^\dagger(\boldsymbol k)e^{-ik\cdot x}\right].
$$

Reality pairs the two terms by Hermitian conjugation. The equal-time [canonical commutation relations](../../../../../canonical-commutation-relation.md) are equivalent to

$$
[a(\boldsymbol k),a^\dagger(\boldsymbol k')]=(2\pi)^3\delta^{(3)}(\boldsymbol k-\boldsymbol k'),
\qquad [a,a]=[a^\dagger,a^\dagger]=0.
$$

For example, the two mixed terms in $[\phi,\pi]$ each supply half the [Dirac delta function](../../../../../dirac-delta-function.md). Thus the normalization $1/\sqrt{2E_{\boldsymbol k}}$ is fixed, not optional. Each independent mode is a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md), with $a$ and $a^\dagger$ its [annihilation operator](../../../../../annihilation-operator.md) and [creation operator](../../../../../creation-operator.md).

Choose the [Fock vacuum](../../../../../fock-vacuum.md) by $a(\boldsymbol k)|0\rangle=0$. Repeated [creation operators](../../../../../creation-operator.md) construct the [bosonic Fock space](../../../../../bosonic-fock-space.md). Substitution into the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) yields

$$
H=\int\frac{d^3\boldsymbol k}{(2\pi)^3}E_{\boldsymbol k}a^\dagger(\boldsymbol k)a(\boldsymbol k)+E_0,
\qquad E_0=\frac V2\int\frac{d^3\boldsymbol k}{(2\pi)^3}E_{\boldsymbol k},
$$

where a finite volume $V$ can be used as a regulator. [Normal ordering](../../../../../normal-ordering.md) sets the flat-space vacuum reference to zero. The spatial [momentum operator](../../../../../momentum-operator.md) is

$$
\boldsymbol P=\int\frac{d^3\boldsymbol k}{(2\pi)^3}\boldsymbol k\,a^\dagger(\boldsymbol k)a(\boldsymbol k).
$$

In particular, $[H,a^\dagger(\boldsymbol k)]=E_{\boldsymbol k}a^\dagger(\boldsymbol k)$ and $[\boldsymbol P,a^\dagger(\boldsymbol k)]=\boldsymbol k\,a^\dagger(\boldsymbol k)$. A one-particle state therefore has positive [energy](../../../../../energy.md), [momentum](../../../../../momentum.md) $\boldsymbol k$, and invariant mass $m$. A scalar field transforms in the trivial [spin](../../../../../spin.md) representation, so its particles have spin zero. Because the field is real there is only one set of oscillators: the particle is its own [antiparticle](../../../../../antiparticle.md), with no distinct conserved particle-minus-antiparticle charge. The free theory does conserve its occupation-number sum, though generic scalar interactions need not.

A momentum eigenstate extends throughout space. A localized particle is described by a superposition such as

$$
|f\rangle=\int\frac{d^3\boldsymbol k}{(2\pi)^3}\,f(\boldsymbol k)a^\dagger(\boldsymbol k)|0\rangle,
\qquad\int\frac{d^3\boldsymbol k}{(2\pi)^3}|f(\boldsymbol k)|^2=1.
$$

Its [wave packet](../../../../../wave-packet.md) evolves through the phase $e^{-iE_{\boldsymbol k}t}$; a narrow packet has [group velocity](../../../../../group-velocity.md) $\boldsymbol v=\boldsymbol k/E_{\boldsymbol k}$, whose magnitude is at most one. Localization and dispersion concern these superpositions, rather than classical trajectories attached to individual field modes.

Relativistic spacetime behavior is encoded by [microcausality](../../../../../microcausality.md). Directly from the oscillator [commutators](../../../../../commutator.md),

$$
[\phi(x),\phi(y)]=\int\frac{d^3\boldsymbol k}{(2\pi)^3\,2E_{\boldsymbol k}}
\left[e^{ik\cdot(x-y)}-e^{-ik\cdot(x-y)}\right].
$$

This is a Lorentz-invariant distribution and vanishes at equal time. Any spacelike separation can be transformed to an equal-time separation, so $[\phi(x),\phi(y)]=0$ for spacelike $x-y$. Thus local operations at spacelike-separated points commute. The vacuum [Wightman function](../../../../../wightman-function.md) need not vanish outside the light cone, but that correlation does not transmit a controllable signal. The [Feynman propagator](../../../../../feynman-propagator.md) is

$$
\langle0|T\phi(x)\phi(y)|0\rangle
=\int\frac{d^4p}{(2\pi)^4}\,\frac{-i\,e^{ip\cdot(x-y)}}{p^2+m^2-i0},
$$

which propagates positive [energy](../../../../../energy.md) forward and negative [energy](../../../../../energy.md) backward in the [time-ordered product](../../../../../time-ordered-product.md). For causal response one uses the [retarded Green function](../../../../../retarded-green-function.md), whose support lies in or on the future light cone.

Finally, commuting [creation operators](../../../../../creation-operator.md) imply

$$
a^\dagger(\boldsymbol k_1)a^\dagger(\boldsymbol k_2)|0\rangle
=a^\dagger(\boldsymbol k_2)a^\dagger(\boldsymbol k_1)|0\rangle.
$$

The multiparticle state is symmetric under the [particle exchange operator](../../../../../particle-exchange-operator.md), which is [Bose statistics](../../../../../bose-einstein-statistics.md). For a normalized single mode, the occupation states are $(a^\dagger)^n|0\rangle/\sqrt{n!}$ with $n=0,1,2,\ldots$: any number of identical [bosons](../../../../../boson.md) can occupy it. There is no [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md) for these particles. This construction agrees with the [Spin-statistics theorem](../../../../../spin-statistics-theorem.md) relating integer [spin](../../../../../spin.md) to bosonic exchange symmetry under relativistic locality and positive-energy assumptions. It demonstrates the required scalar case without assuming that theorem as the quantization prescription.

**The quantized [real scalar field](../../../../../real-scalar-field.md) describes positive-[energy](../../../../../energy.md), mass-$m$, [spin](../../../../../spin.md)-zero [bosons](../../../../../boson.md) that are their own [antiparticles](../../../../../antiparticle.md); commuting [creation operators](../../../../../creation-operator.md) give [Bose statistics](../../../../../bose-einstein-statistics.md), and local field [commutators](../../../../../commutator.md) enforce [microcausality](../../../../../microcausality.md).**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
