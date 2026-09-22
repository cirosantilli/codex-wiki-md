# Finite rectangular barrier matching

↑ **Parent:** [Quantum tunnelling](quantum-tunnelling.md)

Take a [nonrelativistic particle](nonrelativistic-particle.md) of constant [mass](mass.md) $m$ with [energy](energy.md) $E>0$, and choose the same zero of [potential energy](potential-energy.md) on both sides of a [rectangular potential barrier](rectangular-potential-barrier.md):

$$
V(x)=\begin{cases}V_0,&0<x<a,\\0,&x<0\text{ or }x>a,\end{cases}
\qquad V_0>0,\quad a>0.
$$

The equality of the exterior [potential energies](potential-energy.md) matters: it gives the same exterior [wavenumber](wavenumber.md) $k=\sqrt{2mE}/\hbar$ and makes $T=|t|^2$. Here $\hbar=h/(2\pi)$ is the reduced [Planck constant](planck-constant.md). This model has a finite jump in [potential energy](potential-energy.md), no [delta potential](delta-potential.md), and no absorbing term.

For $0<E<V_0$, the [Time-independent Schrödinger equation](time-independent-schrodinger-equation.md) gives the spatial [wavefunction](wave-function.md)

$$
\psi(x)=\begin{cases}
e^{ikx}+re^{-ikx},&x<0,\\
Ae^{\kappa x}+Be^{-\kappa x},&0<x<a,\\
te^{ikx},&x>a,
\end{cases}
\qquad \kappa=\frac{\sqrt{2m(V_0-E)}}{\hbar}.
$$

The full [stationary state](stationary-state.md) is $\Psi(x,t)=\psi(x)e^{-iEt/\hbar}$. We set the incident [probability amplitude](probability-amplitude.md) to one and impose no incoming wave from the right; this [scattering wavefunction](scattering-wavefunction.md) is not a [normalizable wavefunction](normalizable-wavefunction.md). The [tunnelling decay constant](tunnelling-decay-constant.md) $\kappa$ describes [exponential decay](exponential-decay.md), rather than an oscillatory [wavenumber](wavenumber.md) in the barrier. Both [exponential functions](exponential-function.md) are needed on the finite interval: the growing term is not excluded by a condition at infinity.

The [wavefunction](wave-function.md) and its [derivative](derivative.md) are [continuous](continuous-function.md) at each face, giving four linear matching conditions:

$$
\begin{aligned}
1+r&=A+B,&ik(1-r)&=\kappa(A-B),\\
Ae^{\kappa a}+Be^{-\kappa a}&=te^{ika},&
\kappa(Ae^{\kappa a}-Be^{-\kappa a})&=ikte^{ika}.
\end{aligned}
$$

Their solution supplies the [transmission amplitude](transmission-amplitude.md)

$$
t=\frac{e^{-ika}}{\cosh(\kappa a)+i\frac{\kappa^2-k^2}{2k\kappa}\sinh(\kappa a)}.
$$

A short derivation is to use the two right-face equations to express $Ae^{\kappa a}$ and $Be^{-\kappa a}$ in terms of $t$, then substitute into the left-face equations. Taking the squared [modulus](modulus.md) gives the [rectangular barrier transmission probability](rectangular-barrier-transmission-probability.md).

**Table of contents**

- [Tunnelling decay constant](tunnelling-decay-constant.md)
- [Rectangular barrier transmission probability](rectangular-barrier-transmission-probability.md)
  - [Opaque barrier approximation](opaque-barrier-approximation.md)

## ↑ Ancestors (6)

1. [Quantum tunnelling](quantum-tunnelling.md)
2. [Potential barrier](potential-barrier.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
