# Underdamping

↑ **Parent:** [Damping](damping.md)

For $0<\zeta<1$, define the damped [angular frequency](angular-frequency.md) $\omega_{\mathrm d}=\omega_0\sqrt{1-\zeta^2}$. The [initial value problem](initial-value-problem.md) has solution

$$
x(t)=e^{-\zeta\omega_0t}\left[x_0\cos(\omega_{\mathrm d}t)+\frac{v_0+\zeta\omega_0x_0}{\omega_{\mathrm d}}\sin(\omega_{\mathrm d}t)\right].
$$

Every nonzero [underdamped](underdamping.md) response crosses [equilibrium](equilibrium-point-of-a-dynamical-system.md) repeatedly. Its [oscillation period](period-of-an-oscillation.md) is $T_{\mathrm d}=2\pi/\omega_{\mathrm d}$, not $2\pi/\omega_0$. The [amplitude](wave-amplitude.md) envelope decays as $e^{-\zeta\omega_0t}$, but the actual [displacement](displacement.md) also changes sign. The envelope coefficient need not equal $|x_0|$: initial [velocity](velocity.md) fixes the [oscillation phase](phase-waves.md) as well as that coefficient.

## ↑ Ancestors (7)

1. [Damping](damping.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Damping](damping.md)
- [Damping measurement from free decay](damping-measurement-from-free-decay.md)
- [Damping ratio](damping-ratio.md)
- [Logarithmic decrement](logarithmic-decrement.md)
