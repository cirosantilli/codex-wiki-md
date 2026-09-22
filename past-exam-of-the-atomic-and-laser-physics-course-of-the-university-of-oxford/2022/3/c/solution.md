<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the upper-state population lifetime be $T_1=1/\Gamma$, and take the lower [energy level](../../../../energy-level.md) to be stable. [Spontaneous emission](../../../../spontaneous-emission.md) gives survival [probability](../../../../probability.md) $e^{-\Gamma t}$, hence a field or excited-state [probability amplitude](../../../../probability-amplitude.md) proportional to $e^{-\Gamma t/2}e^{-i\omega_0t}$ for $t\geq0$. Its [Fourier transform](../../../../fourier-transform-split.md) at [angular frequency](../../../../angular-frequency.md) $\omega$ is proportional to

$$
\int_0^\infty e^{-\Gamma t/2}e^{i(\omega-\omega_0)t}\,dt
=\frac1{\Gamma/2-i(\omega-\omega_0)}.
$$

The squared modulus therefore has the [Lorentzian line shape](../../../../lorentzian-line-shape.md)

$$
\boxed{L(\omega)=\frac1\pi\frac{\Gamma/2}{(\omega-\omega_0)^2+(\Gamma/2)^2},
\qquad\Delta\omega_{\rm FWHM}=\Gamma=\frac1{T_1}.}
$$

Here $L$ is normalized over the full mathematical [frequency](../../../../frequency.md) axis. The [full width at half maximum](../../../../full-width-at-half-maximum.md) in ordinary [frequency](../../../../frequency.md) is $1/(2\pi T_1)$. If both [energy levels](../../../../energy-level.md) decay, their population decay rates add in the [natural linewidth](../../../../natural-linewidth.md); pure [dephasing](../../../../dephasing-channel.md) adds to the amplitude-decay rate instead.

Impact-regime [pressure broadening](../../../../pressure-broadening.md) provides another example. Independent phase-randomizing collisions with rate $\gamma_c$ give optical correlation proportional to $e^{-\gamma_c|t|}$, whose [Fourier transform](../../../../fourier-transform-split.md) is a [Lorentzian line shape](../../../../lorentzian-line-shape.md) of [full width at half maximum](../../../../full-width-at-half-maximum.md) $2\gamma_c$. This assumes short, uncorrelated impacts: a general static distribution of perturbing fields need not give a [Lorentzian line shape](../../../../lorentzian-line-shape.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
