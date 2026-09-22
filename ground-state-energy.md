# Ground-state energy

↑ **Parent:** [Ground state](ground-state.md)

The ground-state energy $E_0$ is the [energy eigenvalue](energy-eigenvalue-split.md) attained by a [ground state](ground-state.md). For a [self-adjoint operator](self-adjoint-operator.md) $H$ bounded below, distinguish this attained value from the always-defined spectral bottom $E_*=\inf\sigma(H)$. When a [ground state](ground-state.md) exists, $E_0=E_*$. Some usage calls $E_*$ the [ground-state energy](ground-state-energy.md) even when it is unattained; here an unattained bottom is explicitly identified as an [infimum](infimum.md). The [quantum variational principle](quantum-variational-principle.md) states

$$
E_*=\inf_{\substack{\psi\in D(H)\\\|\psi\|=1}}\langle\psi,H\psi\rangle.
$$

Approaching this [infimum](infimum.md) with trial [wavefunctions](wave-function-split.md) does not ensure that a minimizing [wavefunction](wave-function-split.md) exists. [Teschl, Mathematical Methods in Quantum Mechanics, Theorem 2.19](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf).

For the whole-line [free particle](free-particle.md) with mass $m>0$,

$$
H=-\frac{\hbar^2}{2m}\frac{d^2}{dx^2},\qquad \sigma(H)=[0,\infty).
$$

Its [spectrum](spectrum-functional-analysis.md) is continuous and contains no [energy eigenvalues](energy-eigenvalue-split.md) represented by [normalizable wavefunctions](normalizable-wavefunction.md). The [Fourier transform](fourier-transform-split.md) makes $H$ multiplication by $\hbar^2 k^2/(2m)$; a fixed [energy](energy-split.md) restricts $k$ to a set of zero length, on which a nonzero [square-integrable function](square-integrable-function.md) cannot be supported. [Teschl, Mathematical Methods in Quantum Mechanics, section 7.2, Theorem 7.8](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf). An explicit family of normalized [Gaussian wave packets](gaussian-wave-packet.md) demonstrates how the bottom is approached:

$$
\psi_s(x)=(2\pi s^2)^{-1/4}e^{-x^2/(4s^2)},\qquad \langle H\rangle_s=\frac{\hbar^2}{8ms^2}\longrightarrow0\quad(s\longrightarrow\infty).
$$

The formula follows from $\psi_s'=-x\psi_s/(2s^2)$, [integration by parts](integration-by-parts.md), and $\langle x^2\rangle_s=s^2$. Every finite width gives positive [kinetic energy](kinetic-energy.md). At zero [energy](energy-split.md), $H\psi=0$ would require an affine function on the whole line, which is never a nonzero [normalizable wavefunction](normalizable-wavefunction.md). Spreading a [Gaussian wave packet](gaussian-wave-packet.md) indefinitely produces an unattained [infimum](infimum.md), rather than a zero-energy [ground state](ground-state.md).

An additive choice of [energy](energy-split.md) origin changes the numerical [ground-state energy](ground-state-energy.md) without changing the [ground-state subspace](ground-state-subspace.md). For $H'=H+C I$, every [energy eigenvalue](energy-eigenvalue-split.md) becomes $E'=E+C$, while all differences $E_j-E_i$ stay fixed. Time evolution gains only the [global phase](global-phase.md) $e^{-iCt/\hbar}$. This makes excitation costs and spectroscopic differences more intrinsic than the isolated number $E_0$.

**Table of contents**

- [Quantum variational principle](quantum-variational-principle.md)
  - [Excited-state variational constraint](excited-state-variational-constraint.md)
  - [Trial wavefunction](trial-wavefunction.md)
  - [Exponential variational bound for the Yukawa potential](exponential-variational-bound-for-the-yukawa-potential.md)
  - [Power-law quantum virial theorem](power-law-quantum-virial-theorem.md)

## ↑ Ancestors (5)

1. [Ground state](ground-state.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Bose condensation in a three-dimensional harmonic trap](bose-condensation-in-a-three-dimensional-harmonic-trap.md)
- [Bosonic Nambu normal-ordering shift](bosonic-nambu-normal-ordering-shift.md)
- [Density functional variational principle](density-functional-variational-principle.md)
- [Energy eigenvalue](energy-eigenvalue-split.md)
- [Exact variational solution in a two-level system](exact-variational-solution-in-a-two-level-system.md)
- [Excited state](excited-state.md)
- [Exponential variational trial for a square-root half-line well](exponential-variational-trial-for-a-square-root-half-line-well.md)
- [Franck-Hertz experiment](franck-hertz-experiment.md)
- [Gamma-ray energy-network fit](gamma-ray-energy-network-fit.md)
- [Gaussian variational energy for the harmonic oscillator](gaussian-variational-energy-for-the-harmonic-oscillator.md)
- [Ground state](ground-state.md)
- [Ground-state degeneracy](ground-state-degeneracy.md)
- [Ground-state energy](ground-state-energy.md)
- [Infinite square well](infinite-square-well.md)
- [Logarithmic energy gain from a Peierls distortion](logarithmic-energy-gain-from-a-peierls-distortion.md)
- [Mass and range of a nuclear exchange field](mass-and-range-of-a-nuclear-exchange-field.md)
- [Parabolic variational trial for a particle in a box](parabolic-variational-trial-for-a-particle-in-a-box.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018/section-b/b4/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019/section-b/4/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a2/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a2/c/v/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/2/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/34b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/10/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-a/a2/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-a/1/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a1/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/a6/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2013/paper-1/1/b/solution.md)
- [Quantum harmonic oscillator](quantum-harmonic-oscillator-split.md)
- [Quantum variational principle](quantum-variational-principle.md)
- [Trial wavefunction](trial-wavefunction.md)
- [Variational method](variational-method.md)
