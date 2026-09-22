# Standing wave phase and energy

↑ **Parent:** [Standing wave](standing-wave.md)

A stationary [mode shape](mode-shape.md) does not imply absence of [energy](energy-split.md). Write $A=2a$ and $y=A\sin(kx)\cos(\omega t)$. For the ideal [wave equation on a string](wave-equation-on-a-string.md), the [kinetic energy](kinetic-energy.md) and elastic [potential energy](potential-energy.md) per unit reference length add to

$$
e=\frac{\mu}{2}y_t^2+\frac{\tau}{2}y_x^2,
\qquad P=-\tau y_x y_t.
$$

Here $P$ is signed [power](power.md) crossing a position on the string, positive to the right; $e$ is an [energy density](energy-density.md) per length, not per volume. Differentiation and $\mu y_{tt}=\tau y_{xx}$ give the local [conservation of energy](conservation-of-energy.md) identity $\partial_t e+\partial_x P=0$. Substitution into $P$ gives

$$
P(x,t)=\tau A^2k\omega\sin(kx)\cos(kx)\sin(\omega t)\cos(\omega t).
$$

It can be nonzero away from a [node of a standing wave](node-physics.md) or an [antinode](antinode.md), but its time average over an [oscillation period](period-of-an-oscillation.md) is zero. Energy flows locally back and forth even though this pure [standing wave](standing-wave.md) transports no net [energy](energy-split.md) across a section over a complete cycle. At a [node of a standing wave](node-physics.md), $y_t=0$, so [kinetic energy](kinetic-energy.md) density is zero, but $y_x$ need not vanish: elastic [potential energy](potential-energy.md) density can be positive there.

For a fixed-end [normal mode](normal-mode.md), integration over $0\leq x\leq L$ gives

$$
K(t)=\frac{\mu A^2\omega^2L}{4}\sin^2(\omega t),\qquad U(t)=\frac{\tau A^2k^2L}{4}\cos^2(\omega t),\qquad E=K+U=\frac{\mu A^2\omega^2L}{4}.
$$

The last equality uses $\tau k^2=\mu\omega^2$. At a straight-string snapshot, $U=0$ while $K=E$; at an extreme snapshot, $K=0$ while $U=E$. This is [normal-mode energy exchange](normal-mode-energy-exchange.md). A driven real string with [damping](damping.md) requires continuing input [power](power.md) to replace lost [energy](energy-split.md), so a visually stationary pattern does not establish zero average supplied [power](power.md).

## ↑ Ancestors (4)

1. [Standing wave](standing-wave.md)
2. [Mathematical physics](mathematical-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)
