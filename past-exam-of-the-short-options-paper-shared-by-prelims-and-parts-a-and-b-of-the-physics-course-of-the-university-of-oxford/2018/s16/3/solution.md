<h1 id="s16/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use positive [angular frequencies](../../../../angular-frequency.md) and abbreviate $p=\omega_{pe}$, $b=\omega_{ce}$. The left-handed index is $n_L^2=1-p^2/[\omega(\omega+b)]$. It is negative below its positive zero,

$$
\boxed{\omega_L=\frac{\sqrt{b^2+4p^2}-b}{2}.}
$$

For the right-handed mode, $n_R^2=1-p^2/[\omega(\omega-b)]$. Below the [cyclotron resonance](../../../../cyclotron-resonance.md) $0<\omega<b$ its denominator is negative and the index square is positive. Just above the resonance it is negative until

$$
\boxed{\omega_R=\frac{b+\sqrt{b^2+4p^2}}2,\qquad
b<\omega<\omega_R\text{ is the stop band}.}
$$

This is the lossless electron-only cold-plasma model. [Ions](../../../../ion.md), collisions and resonance absorption matter outside its applicable range.

For a whistler with $\omega\ll b$ and $p^2/(\omega b)\gg1$,

$$
k\simeq\frac p{c\sqrt b}\sqrt\omega,\qquad
v_g=\left(\frac{dk}{d\omega}\right)^{-1}
\simeq\frac{2c\sqrt{b\omega}}p.
$$

The travel [time](../../../../time-in-physics.md) through a uniform slab is $t-t_s=Lp\,\omega^{-1/2}/(2c\sqrt b)$. In terms of ordinary [frequency](../../../../frequency.md),

$$
\boxed{\frac{d(f^{-1/2})}{dt}=\frac{2c\sqrt{2\pi b}}{Lp}.}
$$

An arbitrary emission [time](../../../../time-in-physics.md) changes the intercept, not the slope. The original figure labels a dispersion constant $D=81\pm0.5\,\mathrm{Hz^{1/2}\,s}$: it is the reciprocal of the plotted slope, not the slope itself. Therefore

$$
p=\frac{2c\sqrt{2\pi b}}L D,
\qquad b=\frac{eB}{m_e}.
$$

For $B=80$ nT and $L=6.0\times10^7$ m this gives $b\simeq1.41\times10^4\,\mathrm{s^{-1}}$, $p\simeq2.41\times10^5\,\mathrm{s^{-1}}$, and

$$
\boxed{n_e=\frac{\varepsilon_0m_ep^2}{e^2}\simeq1.8\times10^7\,\mathrm{m^{-3}}
\simeq18\,\mathrm{cm^{-3}}.}
$$

The resulting forbidden right-handed [frequency](../../../../frequency.md) width is

$$
\boxed{\Delta f=\frac{\omega_R-b}{2\pi}
=\frac{\sqrt{b^2+4p^2}-b}{4\pi}\simeq3.7\times10^4\,\mathrm{Hz}.}
$$

The lower edge is about $2.24$ kHz and the upper edge about $39.5$ kHz. In the real nonuniform [plasma](../../../../plasma-physics.md), the travel-time coefficient measures a path [integral](../../../../integral-split.md) proportional to $\int\omega_{pe}/\sqrt{\omega_{ce}}\,ds$. The inferred [density](../../../../density.md) is consequently an effective uniform-slab estimate, not a unique local [density](../../../../density.md) at the spacecraft. Uncertainty in the path and [magnetic field](../../../../magnetic-field-split.md) likely exceeds the formal error in $D$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [S16](../../s16.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../split.md)
5. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
