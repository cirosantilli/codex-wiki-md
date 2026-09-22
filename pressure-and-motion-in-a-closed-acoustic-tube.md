# Pressure and motion in a closed acoustic tube

↑ **Parent:** [Kundt's tube](kundt-s-tube.md)

Consider a uniform tube $0\leq x\leq L$ with rigid ends, constant undisturbed [mass density](density.md) $\rho_0$ and [speed of sound](speed-of-sound.md) $c$. Neglect losses and transverse structure. A free [normal mode](normal-mode.md) has

$$
k=\frac{n\pi}{L},\qquad \omega=ck,\qquad n=1,2,\ldots,
$$

and a consistent choice of [sound pressure](sound-pressure.md), [acoustic particle velocity](acoustic-particle-velocity.md) and [acoustic displacement](acoustic-displacement.md) is

$$
\begin{aligned}
p'(x,t)&=P\cos(kx)\cos(\omega t),\\
u(x,t)&=\frac{P}{\rho_0c}\sin(kx)\sin(\omega t),\\
\xi(x,t)&=-\frac{P}{\rho_0c\omega}\sin(kx)\cos(\omega t).
\end{aligned}
$$

Here $P>0$ is a peak [sound pressure](sound-pressure.md). Direct differentiation verifies $\rho_0\partial_tu=-\partial_xp'$ and $\partial_tp'=-\rho_0c^2\partial_xu$, the one-dimensional [linear homentropic acoustic equations](linear-homentropic-acoustic-equations.md). The rigid ends enforce $u=0$ there. A driven experiment only approximates this free-mode geometry; the formulas do not predict a finite resonant [amplitude](wave-amplitude.md) for an undamped driven tube.

The maxima of [sound pressure](sound-pressure.md) amplitude occur at $kx=j\pi$, where [acoustic particle velocity](acoustic-particle-velocity.md) vanishes. The maxima of [acoustic particle velocity](acoustic-particle-velocity.md) amplitude instead occur at $kx=(j+1/2)\pi$, where [sound pressure](sound-pressure.md) vanishes. The two families are displaced by $\lambda/4$, but each family repeats after $\lambda/2$. At a position where both are nonzero, the time dependence is also a quarter cycle apart. Using consecutive maxima of [sound pressure](sound-pressure.md) amplitude therefore gives

$$
\boxed{c=2f d},\qquad f=\frac{\omega}{2\pi},\qquad d=\frac{\lambda}{2}.
$$

The relation also applies to consecutive minima of [sound pressure](sound-pressure.md) amplitude, provided the same family is used throughout. Mixing maxima and minima would halve the spacing and give an erroneous [speed of sound](speed-of-sound.md).

The local [acoustic energy density](acoustic-energy-density.md) is $p'^2/(2\rho_0c^2)+\rho_0u^2/2$. Averaging over one [wave period](wave-period.md) gives $P^2/(4\rho_0c^2)$, independent of $x$. Likewise $\langle p'u\rangle=0$: this ideal [standing wave](standing-wave.md) has no mean longitudinal [acoustic energy flux](acoustic-energy-flux.md), although its [pressure](pressure-split.md) and fluid [velocity](velocity.md) oscillate. Energy transport into a real lossy tube is a different question from the free-mode pattern.

## ↑ Ancestors (6)

1. [Kundt's tube](kundt-s-tube.md)
2. [Linear acoustics](linear-acoustics-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
