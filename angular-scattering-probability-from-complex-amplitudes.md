# Angular scattering probability from complex amplitudes

↑ **Parent:** [Born statistical scattering interpretation](born-statistical-scattering-interpretation.md)

Take [nonrelativistic quantum mechanics](nonrelativistic-quantum-mechanics.md), a short-range interaction, a fixed heavy target, and a common projectile [mass](mass.md) $m$. An incoming [plane wave](plane-wave.md) in atomic state $a$ has unit coefficient. In an open [scattering channel](scattering-channel.md) $i$, the target finishes in a normalized atomic state $\chi_i$, and the projectile has positive [velocity](velocity.md) magnitude $v_i=\hbar k_i/m$. At large distance,

$$
\Psi\sim e^{ik_a z}\chi_a+\sum_{i\,\mathrm{open}}f_{ia}(\Omega)\frac{e^{ik_i r}}r\chi_i,\qquad
\frac{\hbar^2k_i^2}{2m}+\varepsilon_i=\frac{\hbar^2k_a^2}{2m}+\varepsilon_a.
$$

Here $\Omega$ denotes direction, $d\Omega$ is a [solid angle](solid-angle.md) element, and $\varepsilon_i$ is an internal atomic [energy](energy-split.md). Different $\chi_i$ are [orthogonal](orthogonal-vectors.md). The [scattering amplitude](scattering-amplitude.md) $f_{ia}$ has units of length. A closed [scattering channel](scattering-channel.md) has no propagating outgoing [probability current](probability-current.md) at this total [energy](energy-split.md).

The incoming [probability current](probability-current.md) density is $j_{\mathrm{in}}=v_a$. The outgoing radial [probability current](probability-current.md) density in channel $i$ is $j_{r,i}\sim v_i|f_{ia}|^2/r^2$. Multiplying by the area $r^2d\Omega$ and dividing by $j_{\mathrm{in}}$ gives the [differential scattering cross-section](differential-scattering-cross-section.md):

$$
\frac{d\sigma_i}{d\Omega}=\frac{v_i}{v_a}|f_{ia}(\Omega)|^2.
$$

The $r^{-2}$ dilution cancels the detector's area growth. The [velocity](velocity.md) ratio remains: a squared wave coefficient alone is not generally a flux fraction. A [differential scattering cross-section](differential-scattering-cross-section.md) has units of area per [solid angle](solid-angle.md), rather than being a normalized directional [probability density](probability-density.md). For selected scattering events in acceptance $D$, an ideal detector with equal efficiency in all retained channels instead gives

$$
\Pr(i,\Omega\in D\mid\text{selected scattering})
=\frac{\displaystyle\int_D(v_i/v_a)|f_{ia}|^2\,d\Omega}
{\displaystyle\sum_j\int_{\mathrm{selection}}(v_j/v_a)|f_{ja}|^2\,d\Omega}.
$$

The denominator specifies the event selection; it need not equal one square unit of area. Absolute rates require incident flux, target number and detector efficiency in addition to these relative weights. The next finite-mode model normalizes outgoing [probability current](probability-current.md) to one incoming event and predicts event fractions directly.

## ↑ Ancestors (8)

1. [Born statistical scattering interpretation](born-statistical-scattering-interpretation.md)
2. [Born rule](born-rule.md)
3. [Probability amplitude](probability-amplitude.md)
4. [Wave function](wave-function-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
