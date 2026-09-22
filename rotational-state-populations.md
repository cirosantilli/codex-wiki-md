# Rotational state populations

↑ **Parent:** [Rotational spectroscopy](rotational-spectroscopy.md)

For the spin-free [linear rigid rotor](linear-rigid-rotor.md) in [thermal equilibrium](thermal-equilibrium-split.md) at [temperature](temperature-split.md) $T>0$, assume all integer $J\geq0$ are allowed and ignore nuclear-[spin](spin.md) restrictions. Each $J$ level has $2J+1$ [quantum states](quantum-state.md) sharing one [energy eigenvalue](energy-eigenvalue-split.md), an instance of [degenerate energy levels](degenerate-energy-levels.md), so the [Boltzmann distribution](boltzmann-distribution.md) gives

$$
Q_{\rm rot}=\sum_{J=0}^{\infty}(2J+1)e^{-hBJ(J+1)/(k_{\rm B}T)},\qquad
P_J=\frac{(2J+1)e^{-hBJ(J+1)/(k_{\rm B}T)}}{Q_{\rm rot}}.
$$

Here $Q_{\rm rot}$ is a rotational [partition function](canonical-partition-function.md), $h$ the [Planck constant](planck-constant.md), $k_{\rm B}$ the [Boltzmann constant](boltzmann-constant.md), and $B$ a [frequency](frequency.md) in $\mathrm{Hz}$. Thus $hB/(k_{\rm B}T)$ is [dimensionless](dimensionless-quantity.md). The $2J+1$ factor counts [magnetic quantum numbers](magnetic-quantum-number.md); it does not mean that a whole level is one [quantum state](quantum-state.md). For the stipulated $B=5\,\mathrm{GHz}$, the most populated levels are $J=2$ at $3\,\mathrm K$ and $J=7$ at $30\,\mathrm K$.

Population alone is insufficient to predict intensity. In weak, unsaturated absorption, the integrated absorption coefficient includes the transition [frequency](frequency.md), the squared [electric dipole moment](electric-dipole-moment.md) [matrix element](matrix-element.md), and the difference of lower and upper substate populations because [stimulated emission](stimulated-emission.md) returns [energy](energy-split.md) to the field. A pulsed [FTMW spectroscopy](fourier-transform-microwave-spectroscopy.md) signal additionally depends on excitation, [quantum coherence](quantum-coherence-in-a-specified-basis.md), cavity tuning, and receiver response.[Andrei Tokmakoff, §§6.1–6.2, printed pp. 6-2–6-6, equations (6.8)–(6.10), (6.27)–(6.29): population difference and rotational dipole matrix elements](absorption-lineshapes-by-andrei-tokmakoff.md)

For an isotropic sample with [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) along $z$, write $d_z=d\cos\theta$. Normalized [spherical harmonics](spherical-harmonic.md) give

$$
|\langle J+1,M|\cos\theta|J,M\rangle|^2
=\frac{(J+1)^2-M^2}{(2J+1)(2J+3)},\qquad
\sum_{M=-J}^{J}|\langle J+1,M|\cos\theta|J,M\rangle|^2=\frac{J+1}{3}.
$$

The last equality follows from $\sum_{M=-J}^{J}M^2=J(J+1)(2J+1)/3$. Combining this sum with the per-substate [Boltzmann distribution](boltzmann-distribution.md) and subtracting [stimulated emission](stimulated-emission.md) gives relative integrated absorption areas

$$
A_J\propto\frac{\nu_J(J+1)}{Q_{\rm rot}}e^{-hBJ(J+1)/(k_{\rm B}T)}\left(1-e^{-h\nu_J/(k_{\rm B}T)}\right),\qquad \nu_J=2B(J+1).
$$

The common factor includes $d^2/3$ and cancels upon normalization. This formula describes integrated weak absorption in a thermal, spin-free [linear rigid rotor](linear-rigid-rotor.md), not arbitrary peak heights. The example's strongest integrated lines originate at $J=3$ and $J=13$ for $3$ and $30\,\mathrm K$, respectively: they differ from the most populated levels. A missing line can reflect population, coupling, coverage, or sensitivity; it does not prove that the corresponding [quantum state](quantum-state.md) is absent.

**Table of contents**

- [Most populated rotational level](most-populated-rotational-level.md)

## ↑ Ancestors (5)

1. [Rotational spectroscopy](rotational-spectroscopy.md)
2. [Molecular rotation](molecular-rotation.md)
3. [Molecule](molecule-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Most populated rotational level](most-populated-rotational-level.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a3/b/i/solution.md)
- [Rotational spectral line assignment](rotational-spectral-line-assignment.md)
- [Rotational spectroscopy](rotational-spectroscopy.md)
