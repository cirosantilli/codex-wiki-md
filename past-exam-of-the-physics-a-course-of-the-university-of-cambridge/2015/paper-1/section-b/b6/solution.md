<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

**Single travelling wave.** Differentiation of the [plane wave](../../../../../plane-wave.md) gives $\partial_x\psi=ik\psi$, so its [probability current](../../../../../probability-current.md) is

$$
J=\operatorname{Re}\left(\psi^*\frac{\hbar}{im}\partial_x\psi\right)
=\boxed{\frac{\hbar k}{m}|A|^2}.
$$

This is [probability density](../../../../../probability-density.md) times the free-particle velocity $\hbar k/m$.

**Counterpropagating waves.** Remove the common time phase and set $z=B^*Ae^{2ikx}$. Direct multiplication gives

$$
\psi^*\partial_x\psi
=ik\left(|A|^2-|B|^2+z-z^*\right).
$$

Consequently

$$
J=\frac{\hbar k}{m}\operatorname{Re}\left(|A|^2-|B|^2+z-z^*\right)
=\boxed{\frac{\hbar k}{m}\left(|A|^2-|B|^2\right)}.
$$

The [interference](../../../../../interference-wave-propagation.md) term $z-z^*$ is purely imaginary in the last real-part operation. The [probability density](../../../../../probability-density.md) can have [interference fringes](../../../../../interference-fringe.md) even though this net [probability current](../../../../../probability-current.md) is spatially constant.

**Scattering amplitudes.** Locate the step at $x=0$ and first take $E>V$. With $k_1=\sqrt{2mE}/\hbar$ and $k_2=\sqrt{2m(E-V)}/\hbar$, use

$$
\psi_1=e^{ik_1x}+r_a e^{-ik_1x},\qquad
\psi_2=t_a e^{ik_2x}.
$$

The common factor $e^{-iEt/\hbar}$ has been suppressed. A finite step with the same mass on both sides requires continuity of $\psi$ and $\psi'$, giving $1+r_a=t_a$ and $k_1(1-r_a)=k_2t_a$. Hence

$$
\boxed{r_a=\frac{k_1-k_2}{k_1+k_2}
=\frac{\sqrt E-\sqrt{E-V}}{\sqrt E+\sqrt{E-V}}},
\qquad
\boxed{t_a=\frac{2k_1}{k_1+k_2}}.
$$

If $0<E<V$, choose $k_2=i\kappa$, $\kappa=\sqrt{2m(V-E)}/\hbar$, so the transmitted wave decays. The same amplitude formulae continue to hold, but the semi-infinite forbidden region carries no outgoing [probability current](../../../../../probability-current.md): $R=1$ and $T=0$.

**Flux balance.** In the propagating case,

$$
R=|r_a|^2,\qquad
T=\frac{k_2}{k_1}|t_a|^2
=\frac{4k_1k_2}{(k_1+k_2)^2},\qquad R+T=1.
$$

In particular,

$$
J_1=\frac{\hbar k_1}{m}(1-R)
=\frac{\hbar k_2}{m}|t_a|^2=J_2.
$$

The velocity ratio in $T$ is essential: the squared transmission amplitude alone is not the [transmission probability](../../../../../transmission-probability.md) when the two velocities differ.

**Numerical transmission.** The mass cancels from the ratio, and the [energies](../../../../../energy-split.md) can remain in the same [electronvolt](../../../../../electronvolt.md) units:

$$
\boxed{T=\frac{4\sqrt3}{(\sqrt3+1)^2}=0.92820}.
$$

Thus about $92.8\%$ is transmitted and $7.18\%$ reflected, despite the incident [energy](../../../../../energy-split.md) exceeding the step.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
