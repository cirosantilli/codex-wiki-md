# Ground-state energy

↑ **Parent:** [Ground state](ground-state.md)

The ground-state energy $E_0$ is the [energy eigenvalue](energy-eigenvalue.md) attained by a [ground state](ground-state.md). For a [self-adjoint operator](self-adjoint-operator.md) $H$ bounded below, distinguish this attained value from the always-defined spectral bottom $E_*=\inf\sigma(H)$. When a [ground state](ground-state.md) exists, $E_0=E_*$. Some usage calls $E_*$ the [ground-state energy](ground-state-energy.md) even when it is unattained; here an unattained bottom is explicitly identified as an [infimum](infimum.md). The [quantum variational principle](quantum-variational-principle.md) states

$$
E_*=\inf_{\substack{\psi\in D(H)\\\|\psi\|=1}}\langle\psi,H\psi\rangle.
$$

Approaching this [infimum](infimum.md) with trial [wavefunctions](wave-function.md) does not ensure that a minimizing [wavefunction](wave-function.md) exists. [Teschl, Mathematical Methods in Quantum Mechanics, Theorem 2.19](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf).

For the whole-line [free particle](free-particle.md) with mass $m>0$,

$$
H=-\frac{\hbar^2}{2m}\frac{d^2}{dx^2},\qquad \sigma(H)=[0,\infty).
$$

Its [spectrum](spectrum-functional-analysis.md) is continuous and contains no [energy eigenvalues](energy-eigenvalue.md) represented by [normalizable wavefunctions](normalizable-wavefunction.md). The [Fourier transform](fourier-transform.md) makes $H$ multiplication by $\hbar^2 k^2/(2m)$; a fixed [energy](energy.md) restricts $k$ to a set of zero length, on which a nonzero [square-integrable function](square-integrable-function.md) cannot be supported. [Teschl, Mathematical Methods in Quantum Mechanics, section 7.2, Theorem 7.8](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf). An explicit family of normalized [Gaussian wave packets](gaussian-wave-packet.md) demonstrates how the bottom is approached:

$$
\psi_s(x)=(2\pi s^2)^{-1/4}e^{-x^2/(4s^2)},\qquad \langle H\rangle_s=\frac{\hbar^2}{8ms^2}\longrightarrow0\quad(s\longrightarrow\infty).
$$

The formula follows from $\psi_s'=-x\psi_s/(2s^2)$, [integration by parts](integration-by-parts.md), and $\langle x^2\rangle_s=s^2$. Every finite width gives positive [kinetic energy](kinetic-energy.md). At zero [energy](energy.md), $H\psi=0$ would require an affine function on the whole line, which is never a nonzero [normalizable wavefunction](normalizable-wavefunction.md). Spreading a [Gaussian wave packet](gaussian-wave-packet.md) indefinitely produces an unattained [infimum](infimum.md), rather than a zero-energy [ground state](ground-state.md).

An additive choice of [energy](energy.md) origin changes the numerical [ground-state energy](ground-state-energy.md) without changing the [ground-state subspace](ground-state-subspace.md). For $H'=H+C I$, every [energy eigenvalue](energy-eigenvalue.md) becomes $E'=E+C$, while all differences $E_j-E_i$ stay fixed. Time evolution gains only the [global phase](global-phase.md) $e^{-iCt/\hbar}$. This makes excitation costs and spectroscopic differences more intrinsic than the isolated number $E_0$.

**Table of contents**

- [Quantum variational principle](quantum-variational-principle.md)
  - [Exponential variational bound for the Yukawa potential](exponential-variational-bound-for-the-yukawa-potential.md)
  - [Power-law quantum virial theorem](power-law-quantum-virial-theorem.md)

## ↑ Ancestors (5)

1. [Ground state](ground-state.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Bosonic Nambu normal-ordering shift](bosonic-nambu-normal-ordering-shift.md)
- [Energy eigenvalue](energy-eigenvalue.md)
- [Exact variational solution in a two-level system](exact-variational-solution-in-a-two-level-system.md)
- [Excited state](excited-state.md)
- [Franck-Hertz experiment](franck-hertz-experiment.md)
- [Gaussian variational energy for the harmonic oscillator](gaussian-variational-energy-for-the-harmonic-oscillator.md)
- [Ground state](ground-state.md)
- [Ground-state degeneracy](ground-state-degeneracy.md)
- [Ground-state energy](ground-state-energy.md)
- [Infinite square well](infinite-square-well.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/34b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/3/b/ii/solution.md)
- [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)
- [Quantum variational principle](quantum-variational-principle.md)
- [Variational method](variational-method.md)
