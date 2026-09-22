# Photon-number measurement backaction

↑ **Parent:** [Haroche cavity photon nondemolition experiment](haroche-cavity-photon-nondemolition-experiment.md)

An explicit original ideal meter model explains how [photon number](photon-number.md) survives while field [quantum coherence](quantum-coherence-in-a-specified-basis.md) changes. Let $\hat N$ be the [number operator](number-operator.md) and prepare an atomic [qubit](qubit.md) in $|+\rangle=(|e\rangle+|g\rangle)/\sqrt2$. The dispersive [unitary operator](unitary-operator.md)

$$
U=\exp(-i\chi\hat N\otimes\sigma_z/2)
$$

commutes with $\hat N\otimes I$. For a field [quantum superposition](quantum-superposition.md) $\sum_n c_n|n\rangle$, it produces $\sum_n c_n|n\rangle|a_n\rangle$, where $|a_n\rangle=(e^{-in\chi/2}|e\rangle+e^{in\chi/2}|g\rangle)/\sqrt2$. The atomic meter states encode $n$ through relative [quantum phase](quantum-phase.md) and can become [entangled](entangled-state.md) with the field. The second [Ramsey interferometry](ramsey-interferometry.md) pulse and detector turn those correlations into the outcome [probabilities](probability.md) above when $C=1$.

Tracing out the atom multiplies a field [density matrix](density-matrix-split.md) entry $\rho_{nm}$ by $\langle a_m|a_n\rangle=\cos((n-m)\chi/2)$. Hence the [nonselective quantum measurement](nonselective-quantum-measurement.md) preserves every [photon number](photon-number.md) population $\rho_{nn}$ while changing off-diagonal [quantum coherence](quantum-coherence-in-a-specified-basis.md). For $\chi=\pi/2$, coherence between $|0\rangle$ and $|1\rangle$ is multiplied by $1/\sqrt2$ per fresh meter, even with no photons absorbed. Field [quantum phase](quantum-phase.md) information can therefore be disturbed by an energy-preserving probe. No universal self-adjoint phase operator or naive canonical number–phase commutator is needed for this conclusion.

One possible finite-contrast [quantum instrument](quantum-instrument.md) makes the distinction sharper. Define diagonal [Kraus operators](kraus-operator.md) $K_e=\cos((\phi+\chi\hat N)/2)$ and $K_g=\sin((\phi+\chi\hat N)/2)$. After their ideal readout, flip the reported label with [probability](probability.md) $r=(1-C)/2$. The unnormalized selective maps are

$$
\mathcal J_e(\rho)=(1-r)K_e\rho K_e^\dagger+rK_g\rho K_g^\dagger,\qquad
\mathcal J_g(\rho)=rK_e\rho K_e^\dagger+(1-r)K_g\rho K_g^\dagger.
$$

Their [traces](matrix-trace.md) reproduce $L_e,L_g$ on a [Fock state](fock-state.md), and their sum reproduces the displayed dephasing [quantum channel](quantum-channel.md), independently of $r$. At $C=0$ the recorded labels carry no information although the physical meter interaction can still cause [measurement backaction](measurement-backaction.md). This is an illustrative instrument, not a reconstruction of all laboratory imperfections; equal [likelihoods](likelihood-function.md) alone do not determine the disturbance.

## ↑ Ancestors (7)

1. [Haroche cavity photon nondemolition experiment](haroche-cavity-photon-nondemolition-experiment.md)
2. [Quantum nondemolition measurement](quantum-nondemolition-measurement.md)
3. [Measurement in quantum mechanics](quantum-measurement-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
