# Variational method

↑ **Parent:** [Quantum theory](quantum-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variational_method)

The [variational method](variational-method.md) estimates the lowest [energy](energy.md) of a [Quantum Hamiltonian](hamiltonian-quantum-mechanics.md) by choosing a trial [wavefunction](wave-function.md), evaluating its [energy](energy.md), and optimizing the trial parameters. It uses the [quantum variational principle](quantum-variational-principle.md), the [Rayleigh-Ritz variational principle](rayleigh-ritz-variational-principle.md) expressed for [quantum states](quantum-state.md). Let $H$ be a [self-adjoint operator](self-adjoint-operator.md) bounded below, and define $E_0=\inf\sigma(H)$, the bottom of its [spectrum](spectrum-functional-analysis.md). Every normalized admissible trial [quantum state](quantum-state.md) satisfies

$$
E_\psi\geq E_0,\qquad \|\psi\|=1.
$$

When $E_0$ is an [energy eigenvalue](energy-eigenvalue.md), it is the [ground-state energy](ground-state-energy.md); equality holds precisely for a [quantum state](quantum-state.md) in the [ground-state subspace](ground-state-subspace.md). Otherwise the bottom of the [spectrum](spectrum-functional-analysis.md) need not be attained by any normalizable [wavefunction](wave-function.md).

Admissible means finite form energy. Choose a real $b\leq E_0$ and use the shifted [quadratic form of a positive quantum Hamiltonian](quadratic-form-of-a-positive-quantum-hamiltonian.md):

$$
Q(H)=D((H-bI)^{1/2}),\qquad q_H[\psi]=\|(H-bI)^{1/2}\psi\|^2+b\|\psi\|^2,\qquad E_\psi=q_H[\psi].
$$

The form domain $Q(H)$ is independent of this choice of $b$ and can be larger than the [operator domain](operator-domain.md) $D(H)$. For $\psi\in D(H)$, $E_\psi=\langle\psi,H\psi\rangle$ is the usual [expectation value](expectation-value.md); for nonzero unnormalized trials, divide $q_H[\psi]$ by $\|\psi\|^2$ to get the form version of the [Rayleigh quotient](rayleigh-quotient.md). See the [quantum variational principle](quantum-variational-principle.md) for the general domain justification.

Thus each trial [energy](energy.md) is an **upper bound** on $E_0$, and minimizing within a trial family improves that upper bound. It is not a lower bound on $E_0$. The [Gaussian variational energy for the harmonic oscillator](gaussian-variational-energy-for-the-harmonic-oscillator.md) reaches $E_0=1/2$ because its family contains an exact [ground state](ground-state.md). The [exact variational solution in a two-level system](exact-variational-solution-in-a-two-level-system.md) makes the equality condition visible as vanishing excited-state [probability amplitude](probability-amplitude.md).

The method is useful when solving the [Schrödinger equation](schrodinger-equation.md) exactly is difficult but integrals of a trial [wavefunction](wave-function.md) are tractable. Enlarging a trial family cannot increase its optimal [energy](energy.md), although an optimum need not be attained. The beauty is that even an imperfect trial gives a rigorous bound, provided its form energy is computed exactly: numerical integration errors require separate control. The [Gaussian variational estimate for a solvable sextic potential](gaussian-variational-estimate-for-a-solvable-sextic-potential.md) provides an existing example beyond a [quantum harmonic oscillator](quantum-harmonic-oscillator.md).

A short proof explains the direction. With a complete [orthonormal eigenbasis](orthonormal-eigenbasis.md) of [energy eigenstates](energy-eigenstate.md), write $\psi=\sum_n c_n\phi_n$, where $H\phi_n=E_n\phi_n$ and $\sum_n|c_n|^2=1$. Then

$$
E_\psi-E_0=\sum_n|c_n|^2(E_n-E_0)\geq0.
$$

This is a [weighted mean](weighted-arithmetic-mean.md) of nonnegative [energy](energy.md) differences; equality requires every occupied [energy eigenstate](energy-eigenstate.md) to have [energy](energy.md) $E_0$. [Barton Zwiebach, Wave Mechanics, MIT 8.05, 2013, §5, pp. 18–20](https://ocw.mit.edu/courses/8-05-quantum-physics-ii-fall-2013/61bc31b8d8bf0680c322733910a71aa0_MIT8_05F13_Chap_01.pdf). For [continuous spectrum](continuous-spectrum.md), the [spectral theorem](spectral-theorem.md) replaces the sum by an integral against the [scalar spectral measure](scalar-spectral-measure.md) of $\psi$, with the same nonnegative integrand. This proves the bound without assuming an [orthonormal eigenbasis](orthonormal-eigenbasis.md) exists.

The historical setting predates [quantum mechanics](quantum-mechanics-split.md): Rayleigh's _The Theory of Sound_, volume I, appeared in 1877, and Ritz's paper on solving variational problems of mathematical physics appeared in volume 135 of Crelle's journal, catalogued by its publisher as 1909, pp. 1–61. These are original works associated with the [Rayleigh-Ritz method](rayleigh-ritz-method.md); the dates here identify the publications rather than assert priority. [Lord Rayleigh, The Theory of Sound, volume I, 1877](https://archive.org/details/theorysound06raylgoog); [Walter Ritz, Über eine neue Methode zur Lösung gewisser Variationsprobleme der mathematischen Physik, original article and publisher metadata](https://doi.org/10.1515/crll.1909.135.1).

**Table of contents**

- [Gaussian variational energy for the harmonic oscillator](gaussian-variational-energy-for-the-harmonic-oscillator.md)
- [Nodeless theorem for a one-dimensional ground state](nodeless-theorem-for-a-one-dimensional-ground-state.md)
- [Exact ground state of a solvable sextic potential](exact-ground-state-of-a-solvable-sextic-potential.md)
- [Gaussian variational estimate for a solvable sextic potential](gaussian-variational-estimate-for-a-solvable-sextic-potential.md)
- [Ground-state energy monotonicity under potential ordering](ground-state-energy-monotonicity-under-potential-ordering.md)
- [Quantum virial identity from scaling](quantum-virial-identity-from-scaling.md)
  - [Fall to the centre for a supercritical inverse-power potential](fall-to-the-centre-for-a-supercritical-inverse-power-potential.md)
- [Exact variational solution in a two-level system](exact-variational-solution-in-a-two-level-system.md)
  - [Level repulsion in a two-level Hamiltonian](level-repulsion-in-a-two-level-hamiltonian.md)

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Exact variational solution in a two-level system](exact-variational-solution-in-a-two-level-system.md)
- [Gaussian variational energy for the harmonic oscillator](gaussian-variational-energy-for-the-harmonic-oscillator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/36e/a/solution.md)
- [Variational method](variational-method.md)
