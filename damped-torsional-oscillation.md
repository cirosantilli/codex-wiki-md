# Damped torsional oscillation

↑ **Parent:** [Torsion constant](torsion-constant.md)

A [damped torsional oscillation](damped-torsional-oscillation.md) is rotation about a fiber's fixed reference orientation with a restoring [torque](torque.md) and dissipative [torque](torque.md). In the ideal viscous model, [damping](damping.md) contributes $-b\dot\theta$ with constant $b\geq0$. This is a rotational [damped harmonic oscillator](damped-harmonic-oscillator.md). For known constant [moment of inertia](moment-of-inertia.md) $I$ and [torsion constant](torsion-constant.md) $\kappa$, define $\gamma=b/(2I)$. In the oscillatory regime $\gamma^2<\kappa/I$,

$$
\theta(t)=A e^{-\gamma t}\cos(\omega_dt+\varphi),\qquad \omega_d^2=\frac\kappa I-\gamma^2,\qquad T_d=\frac{2\pi}{\omega_d}.
$$

$A$ and $\varphi$ are set by the initial state. Successive positive peaks measured from the same [equilibrium](equilibrium-point-of-a-dynamical-system.md) have magnitudes $p_n$ and $p_{n+1}$; their ratio gives $\delta=\ln(p_n/p_{n+1})=\gamma T_d$. Consequently a measured damped [oscillation period](period-of-an-oscillation.md) and decay together recover

$$
\boxed{\kappa=I\left[\left(\frac{2\pi}{T_d}\right)^2+\gamma^2\right]=\frac I{T_d^2}(4\pi^2+\delta^2).}
$$

Using only $4\pi^2I/T_d^2$ underestimates the [torsion constant](torsion-constant.md) in this model. The toy curve in [torsion constant](torsion-constant.md) sets $I=2.0\times10^{-6}\,\mathrm{kg\,m^2}$, $\kappa=1.0\times10^{-8}\,\mathrm{N\,m/rad}$, and $\gamma=0.020\,\mathrm{s^{-1}}$. It gives $T_0\simeq88.86\,\mathrm s$, $T_d\simeq92.64\,\mathrm s$, and $\delta\simeq1.853$. Ignoring the decay recovers $9.2\times10^{-9}\,\mathrm{N\,m/rad}$, an $8\%$ underestimate; including it recovers the stipulated [torsion constant](torsion-constant.md).

These equations assume a single rotational mode, a stationary zero, [linear elasticity](linear-elasticity.md), and viscous [damping](damping.md). Internal fiber losses need not behave as a constant viscous coefficient: Fleischer and colleagues model their precision apparatus using a loss angle. Their response is evidence for specifying a damping model, not for applying the viscous correction universally. [Fleischer et al. (2022), §I, equation (1): thermal torque noise and internal damping represented by a loss angle](https://arxiv.org/pdf/2206.02890)

## ↑ Ancestors (6)

1. [Torsion constant](torsion-constant.md)
2. [Torsion balance](torsion-balance.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Damped torsional oscillation](damped-torsional-oscillation.md)
- [Torsion constant](torsion-constant.md)
