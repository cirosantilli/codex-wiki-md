<h1 id="section-b/b7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For [underdamping](../../../../../../underdamping.md), the general response is a free transient plus a particular driven response. Use the paper's $e^{i\omega t}$ convention. The steady displacement [complex amplitude](../../../../../../complex-amplitude.md) is

$$
x_0=\frac{F_0}{k-m\omega^2+ib\omega}.
$$

Thus

$$
\boxed{x(t)=e^{-\gamma t}[C\cos(\omega_dt)+D\sin(\omega_dt)]
+\operatorname{Re}\!\left[\frac{F_0e^{i\omega t}}{k-m\omega^2+ib\omega}\right].}
$$

Here $\gamma=b/(2m)$, $\omega_d=\sqrt{k/m-\gamma^2}$ and the real constants $C,D$ enforce the initial conditions. For a real positive $F_0$, the steady term is $|x_0|\cos(\omega t-\phi)$, where

$$
|x_0|=\frac{F_0}{\sqrt{(k-m\omega^2)^2+b^2\omega^2}},\qquad
\phi=\operatorname{atan2}(b\omega,k-m\omega^2).
$$

For light [damping](../../../../../../damping.md), $\omega_d\simeq\omega_0$ and the transient decays slowly compared with an oscillation. The two-argument phase convention makes the displacement lag evolve from approximately zero below resonance through $\pi/2$ near $\omega_0$ to approximately $\pi$ far above it.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
