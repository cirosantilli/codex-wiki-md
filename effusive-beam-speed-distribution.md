# Effusive beam speed distribution

↑ **Parent:** [Molecular beam](molecular-beam.md)

Which [speed distribution](speed-distribution.md) does an arrival counter measure? Suppose an equilibrium, nonrelativistic [ideal gas](ideal-gas-split.md) escapes by [effusion](effusion.md) through a thin opening into [vacuum](vacuum.md). The opening is small compared with the [mean free path](mean-free-path.md); the reservoir remains at [temperature](temperature-split.md) $T$. Let $f(v)$ denote its normalized [Maxwell speed distribution](maxwell-speed-distribution.md), with [mass](mass.md) $m$ and $a=m/(2k_BT)$:

$$
f(v)=\frac{4a^{3/2}}{\sqrt\pi}v^2e^{-av^2},\qquad v>0.
$$

At a given direction toward the opening, the number crossing per unit time is proportional to the normal component $v\cos\theta$. Integrating over a fixed accepted cone contributes an angular factor independent of $v$. Thus the normalized [probability density function](probability-density-function.md) for speeds among arriving particles is

$$
\boxed{g(v)=\frac{vf(v)}{\langle v\rangle}=2a^2v^3e^{-av^2}}.
$$

Its [integral](integral-split.md) is one because $\int_0^\infty v^3e^{-av^2}\,dv=1/(2a^2)$. The reservoir [mode](mode-statistics.md) is $v=\sqrt{2k_BT/m}$; the arrival [mode](mode-statistics.md) is $\sqrt{3k_BT/m}$. Faster particles get more opportunities to cross the opening. This is a selection effect, not heating after emission.

Specify the observable before applying the formula. An instantaneous count in a fixed segment of the beam weights the arrival flux by the time spent there, proportional to $1/v$; in this ideal model its normalized speed law returns to $f(v)$. A detector's speed-dependent efficiency, source [collisions](collision.md) or a velocity selector changes the arriving law again. **Counting arrivals and counting particles currently present are different measurements.**

## ↑ Ancestors (4)

1. [Molecular beam](molecular-beam.md)
2. [Experimental apparatus](experimental-apparatus.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Gravity deflection of an atomic beam](gravity-deflection-of-an-atomic-beam.md)
- [Molecular beam](molecular-beam.md)
- [Speed distribution](speed-distribution.md)
