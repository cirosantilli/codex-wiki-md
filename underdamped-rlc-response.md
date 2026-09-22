# Underdamped RLC response

↑ **Parent:** [Series RLC circuit](series-rlc-circuit.md)

An [underdamped RLC response](underdamped-rlc-response.md) is a free [series RLC circuit](series-rlc-circuit.md) response with $0<R<2\sqrt{L/C}$, equivalently $0<\alpha<\omega_0$. Its [characteristic roots](characteristic-root-of-a-constant-coefficient-differential-equation.md) are $-\alpha\pm\mathrm{i}\omega_d$, and its general [electric charge](electric-charge-split.md) is

$$
q(t)=e^{-\alpha t}\left(A\cos(\omega_dt)+B\sin(\omega_dt)\right).
$$

For [initial conditions](initial-condition.md) $q(0)=q_0$, $i(0)=0$,

$$
q(t)=q_0e^{-\alpha t}\left(\cos(\omega_dt)+\frac\alpha{\omega_d}\sin(\omega_dt)\right),\qquad
i(t)=-\frac{q_0\omega_0^2}{\omega_d}e^{-\alpha t}\sin(\omega_dt).
$$

In the dimensionless example $\omega_0=1$, $\alpha=0.5$, the ringing [angular frequency](angular-frequency.md) is $\omega_d=\sqrt3/2\approx0.866025$, below the driven [electric current](electric-current.md) [resonance](resonance.md) at $\omega_0=1$. The [electric charge](electric-charge-split.md) first crosses zero at $t=4\pi/(3\sqrt3)\approx2.41840$ and reaches its first negative extremum at $t=2\pi/\sqrt3\approx3.62760$, where $q/q_0=-e^{-\pi/\sqrt3}\approx-0.163034$.

The sinusoidal factor changes sign while its envelope decays as $e^{-\alpha t}$. The total [energy](energy-split.md) follows the exact balance $E'=-Ri^2$, rather than a pure [exponential decay](exponential-decay.md) at every instant; in particular, its rate of loss is zero whenever $i=0$. As $\alpha\to0$, the displayed solution tends to the lossless [harmonic oscillator](simple-harmonic-motion.md) $q=q_0\cos(\omega_0t)$. As $\alpha\to\omega_0$ from below, $\sin(\omega_dt)/\omega_d\to t$, recovering the [critically damped RLC response](critically-damped-rlc-response.md) continuously. The [overdamped RLC response](overdamped-rlc-response.md) reaches the same limit through $\sinh(\beta t)/\beta\to t$.

## ↑ Ancestors (7)

1. [Series RLC circuit](series-rlc-circuit.md)
2. [RLC circuit](rlc-circuit.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Critically damped RLC response](critically-damped-rlc-response.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/5c/c/ii/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2/section-a/3/solution.md)
- [Resonant series RLC response](resonant-series-rlc-response.md)
- [Series RLC circuit](series-rlc-circuit.md)
- [Underdamped RLC response](underdamped-rlc-response.md)
