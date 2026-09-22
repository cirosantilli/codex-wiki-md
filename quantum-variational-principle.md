# Quantum variational principle

↑ **Parent:** [Ground-state energy](ground-state-energy.md)

The [quantum variational principle](quantum-variational-principle.md) estimates the lowest energy by choosing a trial [wavefunction](wave-function-split.md) and computing its [expectation value](expectation-value.md), without solving the [Schrödinger equation](schrodinger-equation.md) exactly. Minimizing over a manageable family of trial [wavefunctions](wave-function-split.md) gives an upper bound; enlarging that family can improve the estimate.

Let $H$ be a [self-adjoint operator](self-adjoint-operator.md) bounded below, and put $E_*=\inf\sigma(H)$. For $\|\psi\|=1$ in its [operator domain](operator-domain.md) $D(H)$,

$$
\langle\psi,H\psi\rangle\geq E_*.
$$

Trial states may also lie in the form domain $Q(H)=D((H-bI)^{1/2})$, where $b\leq E_*$. Then use the [quadratic form of a positive quantum Hamiltonian](quadratic-form-of-a-positive-quantum-hamiltonian.md) shifted by $b$:

$$
q_H[\psi]=\|(H-bI)^{1/2}\psi\|^2+b\|\psi\|^2\geq E_*\|\psi\|^2.
$$

This extends the [expectation value](expectation-value.md) beyond $D(H)$ without requiring $H\psi$ to exist. Equality for a normalized state holds exactly in the [energy eigenspace](energy-eigenspace.md) at $E_*$, if that [eigenvalue](eigenvalue.md) exists. [Gerald Teschl, Mathematical Methods in Quantum Mechanics, Theorem 2.19 and equations (3.50)–(3.51)](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf).

A short proof makes the direction of the bound memorable. If $H$ has a complete [orthonormal basis](orthonormal-basis.md) of [energy eigenstates](energy-eigenstate.md) $\phi_n$, write

$$
\psi=\sum_n c_n\phi_n,\qquad H\phi_n=E_n\phi_n,\qquad \sum_n|c_n|^2=1.
$$

The [expectation value](expectation-value.md) is a weighted average of allowed energies:

$$
q_H[\psi]-E_*=\sum_n|c_n|^2(E_n-E_*)\geq0.
$$

Equality requires every occupied [energy eigenstate](energy-eigenstate.md) to have energy $E_*$. [Barton Zwiebach, MIT 8.05 Wave Mechanics, section 5, Variational Principle](https://live.ocw.mit.edu/courses/8-05-quantum-physics-ii-fall-2013/61bc31b8d8bf0680c322733910a71aa0_MIT8_05F13_Chap_01.pdf). With [continuous spectrum](continuous-spectrum.md), the [spectral theorem](spectral-theorem.md) replaces the sum by an integral against the [scalar spectral measure](scalar-spectral-measure.md); the same nonnegative-difference argument works.

For an unnormalized trial [wavefunction](wave-function-split.md), divide by its squared norm: $R_H[\psi]=q_H[\psi]/\|\psi\|^2$ is the form version of the [Rayleigh quotient](rayleigh-quotient.md). The [quantum variational principle](quantum-variational-principle.md) supplies an upper bound on $E_*$; it supplies neither a lower bound on $E_*$ nor, by itself, a guarantee that a [bound state](bound-state.md) exists.

To see the method at work, choose the real [Gaussian wave packet](gaussian-wave-packet.md)

$$
\psi_a(x)=\left(\frac a\pi\right)^{1/4}e^{-ax^2/2},\qquad a>0,\qquad x\in\mathbb R.
$$

The [Gaussian integral](gaussian-integral.md) gives [wavefunction normalization](wavefunction-normalization.md) and the two useful position averages:

$$
\int_{\mathbb R}|\psi_a|^2\,dx=1,\qquad \langle x^2\rangle_a=\frac1{2a},\qquad \langle x^4\rangle_a=\frac3{4a^2}.
$$

Thus its position [probability density](probability-density.md) is a [normal distribution](normal-distribution.md) with [standard deviation](standard-deviation.md) $1/\sqrt{2a}$: large $a$ means narrow confinement. In units $\hbar=m=1$, [integration by parts](integration-by-parts.md) and $\psi_a'=-ax\psi_a$ give the [kinetic energy](kinetic-energy.md)

$$
\langle T\rangle_a=\frac12\int_{\mathbb R}|\psi_a'|^2\,dx=\frac{a^2}2\langle x^2\rangle_a=\frac a4.
$$

These smooth, rapidly decaying trial [wavefunctions](wave-function-split.md) belong to the [operator domains](operator-domain.md) of both polynomial [Quantum Hamiltonians](hamiltonian-quantum-mechanics.md) below. Narrowing the [Gaussian wave packet](gaussian-wave-packet.md) increases its [kinetic energy](kinetic-energy.md); widening it increases the [potential energy](potential-energy.md) in either confining potential.

For the [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md), take $\hbar=m=\omega=1$:

$$
H_{\mathrm{ho}}=-\frac12\frac{d^2}{dx^2}+\frac{x^2}2,\qquad E_{\mathrm{ho}}(a)=\frac a4+\frac1{4a}.
$$

The trial values at $a=1/2,1,2$ are respectively $0.625,0.5,0.625$. The [derivative](derivative.md) $E_{\mathrm{ho}}'(a)=(1-a^{-2})/4$ changes sign at $a=1$, where [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md) are both $1/4$. Here the trial family contains an exact [ground state](ground-state.md):

$$
H_{\mathrm{ho}}\psi_1=\frac12\psi_1,\qquad E_0=\frac12.
$$

The [zero-point energy](zero-point-energy.md) remains positive even at the best width. For comparison, removing the potential leaves $E(a)=a/4\to0$ as $a\to0$: the free [Quantum Hamiltonian](hamiltonian-quantum-mechanics.md) on the line has spectral bottom zero but no normalizable zero-energy [energy eigenstate](energy-eigenstate.md). A sequence of ever broader trial [wavefunctions](wave-function-split.md) need not approach an actual [bound state](bound-state.md).

<a id="image-gaussian-trial-widths-and-the-kinetic-potential-energy-tradeoff"></a>
![](quantum-variational-gaussian.png)

**[Figure 13](#image-gaussian-trial-widths-and-the-kinetic-potential-energy-tradeoff). Gaussian trial widths and the kinetic–potential energy tradeoff**. Normalized [Gaussian wave packets](gaussian-wave-packet.md) with $a=1/2,1,2$ have different position [probability densities](probability-density.md). The bars show the competing [kinetic energy](kinetic-energy.md) $a/4$ and harmonic [potential energy](potential-energy.md) $1/(4a)$; their sum is smallest at $a=1$.

For a pure [quartic oscillator](quartic-oscillator.md), keep $\hbar=m=1$ and set the quartic coefficient to one:

$$
H_4=-\frac12\frac{d^2}{dx^2}+x^4,\qquad E_4(a)=\frac a4+\frac3{4a^2}.
$$

The trial values at $a=1,2,3$ are respectively $1,0.6875,0.833333\ldots$. Setting the [derivative](derivative.md) to zero gives

$$
E_4'(a)=\frac14-\frac3{2a^3}=0,\qquad a_{\mathrm{opt}}=6^{1/3}\approx1.817121.
$$

The sign of this [derivative](derivative.md) changes from negative to positive at the optimum, giving the smallest energy within this [Gaussian wave packet](gaussian-wave-packet.md) family:

$$
E_{0,4}\leq\min_{a>0}E_4(a)=\frac38\,6^{1/3}\approx0.681420.
$$

At this width, $\langle T\rangle\approx0.454280$ and $\langle V\rangle\approx0.227140$, so $2\langle T\rangle=4\langle V\rangle$, as expected from the [power-law quantum virial theorem](power-law-quantum-virial-theorem.md) for a scale-optimized trial [wavefunction](wave-function-split.md). The number $0.681420$ is an upper estimate of the [ground-state energy](ground-state-energy.md), not an asserted exact [energy eigenvalue](energy-eigenvalue-split.md). Indeed,

$$
\frac{H_4\psi_a}{\psi_a}=x^4-\frac{a^2x^2}2+\frac a2
$$

depends on $x$ for every $a>0$, so no member of this trial family is an [energy eigenstate](energy-eigenstate.md). Nevertheless, a single width parameter already turns a difficult [Schrödinger equation](schrodinger-equation.md) into a useful, explicit energy estimate.

<a id="image-energy-landscapes-for-harmonic-and-quartic-gaussian-trials"></a>
![](quantum-variational-energy-landscape.png)

**[Figure 14](#image-energy-landscapes-for-harmonic-and-quartic-gaussian-trials). Energy landscapes for harmonic and quartic Gaussian trials**. The [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) reaches its exact [ground-state energy](ground-state-energy.md) $1/2$ at $a=1$. The pure [quartic oscillator](quartic-oscillator.md) has a [Gaussian wave packet](gaussian-wave-packet.md) optimum at $a=6^{1/3}$ giving only the upper bound $E_{0,4}\leq0.681420$. Dashed curves separate [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md).

**Table of contents**

- [Excited-state variational constraint](excited-state-variational-constraint.md)
- [Trial wavefunction](trial-wavefunction.md)
- [Exponential variational bound for the Yukawa potential](exponential-variational-bound-for-the-yukawa-potential.md)
- [Power-law quantum virial theorem](power-law-quantum-virial-theorem.md)

## ↑ Ancestors (6)

1. [Ground-state energy](ground-state-energy.md)
2. [Ground state](ground-state.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (26)

- [Compactly supported linear trial for hydrogen](compactly-supported-linear-trial-for-hydrogen.md)
- [Exponential variational trial for a square-root half-line well](exponential-variational-trial-for-a-square-root-half-line-well.md)
- [Ground state](ground-state.md)
- [Ground-state energy](ground-state-energy.md)
- [Helium variational effective charge](helium-variational-effective-charge.md)
- [Mass and range of a nuclear exchange field](mass-and-range-of-a-nuclear-exchange-field.md)
- [Parabolic variational trial for a particle in a box](parabolic-variational-trial-for-a-particle-in-a-box.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019/section-b/4/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a2/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a2/a/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a2/c/v/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a2/c/vi/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-1/a2/a/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-1/a1/b/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-b/33/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-b/33/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-b/33/c/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-b/33/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/33c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/34b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/10/solution.md)
- [Quantum harmonic oscillator](quantum-harmonic-oscillator-split.md)
- [Quantum variational principle](quantum-variational-principle.md)
- [Variational method](variational-method.md)
