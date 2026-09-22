# Energy transfer after an impulse in two weakly coupled oscillators

↑ **Parent:** [Coupled oscillator](coupled-oscillator.md)

Consider identical [harmonic oscillators](simple-harmonic-motion.md) with unit [mass](mass.md), natural [angular frequency](angular-frequency.md) $\omega_0>0$, and positive coupling $\kappa\ll\omega_0^2$:

$$
\ddot x_1+\omega_0^2x_1+\kappa(x_1-x_2)=0,\qquad
\ddot x_2+\omega_0^2x_2+\kappa(x_2-x_1)=0.
$$

An initial [impulse](impulse.md) on the first gives $x_1(0)=x_2(0)=\dot x_2(0)=0$ and $\dot x_1(0)=v$. The [normal mode coordinates](normal-coordinate.md) $u=x_1+x_2$ and $w=x_1-x_2$ have [angular frequencies](angular-frequency.md) $\omega_0$ and $\omega_a=\sqrt{\omega_0^2+2\kappa}$. Solving their [initial value problems](initial-value-problem.md) proves

$$
x_1=\frac v2\left(\frac{\sin\omega_0t}{\omega_0}+\frac{\sin\omega_at}{\omega_a}\right),\qquad
x_2=\frac v2\left(\frac{\sin\omega_0t}{\omega_0}-\frac{\sin\omega_at}{\omega_a}\right).
$$

Let $\Delta=\omega_a-\omega_0\sim\kappa/\omega_0$. To leading order in $\kappa/\omega_0^2$, sum-to-product identities give the displacement [amplitude](wave-amplitude.md) envelopes $(|v|/\omega_0)|\cos(\Delta t/2)|$ and $(|v|/\omega_0)|\sin(\Delta t/2)|$. Thus the first nearly complete [energy](energy-split.md) transfer occurs at $\pi/\Delta$, and localization returns at $2\pi/\Delta$. More precisely, at $t=\pi/\Delta$, the first [oscillator](oscillator.md) has exactly zero [velocity](velocity.md) and residual [displacement](displacement.md) $\tfrac v2(1/\omega_0-1/\omega_a)\sin(\omega_0t)$, of order $|v|\kappa/\omega_0^3$.

Here transferred [energy](energy-split.md) means [kinetic energy](kinetic-energy.md) plus the uncoupled quadratic [potential energy](potential-energy.md); the coupling [potential energy](potential-energy.md) is relatively small. The fast phase need not make the receiving [oscillator](oscillator.md) pass through zero [displacement](displacement.md) at the transfer time. Expanding $\Delta t$ as small is invalid on the transfer scale $t=O(1/\kappa)$. This lemma complements [absolute and signed beat envelopes](absolute-and-signed-beat-envelopes.md) by keeping that slow phase.

## ↑ Ancestors (6)

1. [Coupled oscillator](coupled-oscillator.md)
2. [Oscillator](oscillator.md)
3. [Oscillation](oscillation.md)
4. [Wave](wave-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-classical-mechanics-course-of-the-university-of-oxford/2023/1/c/solution.md)
