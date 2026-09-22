# Electric-dipole excitation by a passing ion

↑ **Parent:** [Coulomb excitation](coulomb-excitation.md)

In the straight-trajectory dipole model, retain the Coulomb-coupling convention of $V(t)=Ze^2(bx+vty)/(b^2+v^2t^2)^{3/2}$. In SI units the coupling denoted $e^2$ here is $e^2/(4\pi\epsilon_0)$. First-order [time-dependent perturbation theory](time-dependent-perturbation-theory.md) expresses a transition through the [Fourier transform](fourier-transform-split.md) of this pulse at the transition angular frequency.

For positive $\omega$ put $\beta=\omega b/v$. The two Cartesian pulse transforms are

$$
I_x=\int_{-\infty}^{\infty}\frac{b e^{i\omega t}}{(b^2+v^2t^2)^{3/2}}dt=\frac{2\beta K_1(\beta)}{bv},\qquad
I_y=\int_{-\infty}^{\infty}\frac{vt e^{i\omega t}}{(b^2+v^2t^2)^{3/2}}dt=\frac{2i\beta K_0(\beta)}{bv},
$$

where $K_\nu$ is a [Modified Bessel function of the second kind](modified-bessel-function-of-the-second-kind.md). One may derive these from the Fourier transform of $(1+s^2)^{-1/2}$, differentiating in its scale and integrating its spatial derivative by parts. For $\beta\ll1$, $\beta K_1(\beta)\to1$ while $\beta K_0(\beta)\to0$, so the transverse impulse gives the probability in the title. If the $x$ [matrix element](matrix-element.md) vanishes, the smaller longitudinal term can be the leading nonzero contribution.

The conditions include $b$ large compared with the atomic extent for the [electric-dipole approximation](electric-dipole-approximation.md), a small total transition [probability](probability.md) for first-order theory, and a collision time $b/v$ short compared with $1/|\omega|$. Large $\beta$ instead gives exponentially suppressed excitation in this model through the large-argument behavior of $K_\nu$.

## ↑ Ancestors (6)

1. [Coulomb excitation](coulomb-excitation.md)
2. [Collective nuclear model](collective-nuclear-model.md)
3. [Atomic nucleus](atomic-nucleus-split.md)
4. [Nuclear physics](nuclear-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019/section-b/6/solution.md)
