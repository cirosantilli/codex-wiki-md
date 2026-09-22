<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take positive [heat](../../../../../heat-split.md) flux upwards, along increasing $z$, and denote [thermal conductivity](../../../../../thermal-conductivity.md) by $k$. [Fourier's law](../../../../../fourier-s-law.md) gives $q_s=-kT_z|_{z=a}$. Since $\cos(n\pi)=(-1)^n$, [differentiation](../../../../../differentiation.md) of the literal printed expression gives

$$
\boxed{q_{s,\rm printed}(t)=\frac{k\Delta T}{a}
\left[1-2\sum_{n=1}^\infty e^{-n^2t/\tau_0}\right].}
$$

Its negative young-age flux is another sign of the unphysical initial profile. For the explicitly corrected hot initial plate, the [surface heat flux of a cooling plate](../../../../../surface-heat-flux-of-a-cooling-plate.md) is instead

$$
\boxed{q_s(t)=\frac{k\Delta T}{a}
\left[1+2\sum_{n=1}^\infty e^{-n^2t/\tau_0}\right].}
$$

The old-age limit is $k\Delta T/a$. For $t\ll\tau_0$, replacing the Gaussian sum by its leading [integral](../../../../../integral-split.md) gives $q_s\sim k\Delta T/\sqrt{\pi\kappa t}$, recovering the [half-space cooling model](../../../../../half-space-cooling-model.md). Neither $k$ nor $\kappa$ is numerically specified, so the age-dependent flux remains symbolic as requested.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../split.md)
6. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
