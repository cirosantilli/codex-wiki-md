<h1 id="section-b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Count wavevectors in a large volume with [periodic boundary conditions](../../../../../periodic-boundary-conditions.md). One spin-degenerate spherical band supplies

$$
\frac{N(k)}{\mathcal V}=\frac{2}{(2\pi)^3}\frac{4\pi k^3}{3}=\frac{k^3}{3\pi^2},\qquad
\frac1{\mathcal V}\frac{dN}{dk}=\frac{k^2}{\pi^2}.
$$

For the [conduction band](../../../../../conduction-band.md), $k=\sqrt{2m_e^*(\epsilon-\epsilon_c)}/\hbar$ and $dk/d\epsilon=m_e^*/(\hbar^2k)$. Transforming the state count to energy gives

$$
\boxed{g_e(\epsilon)=\frac1{2\pi^2}\left(\frac{2m_e^*}{\hbar^2}\right)^{3/2}\sqrt{\epsilon-\epsilon_c},\qquad\epsilon\geq\epsilon_c.}
$$

For the [valence band](../../../../../valence-band.md) use $|dk/d\epsilon|=m_h^*/(\hbar^2k)$ and $k=\sqrt{2m_h^*(\epsilon_v-\epsilon)}/\hbar$, obtaining

$$
\boxed{g_h(\epsilon)=\frac1{2\pi^2}\left(\frac{2m_h^*}{\hbar^2}\right)^{3/2}\sqrt{\epsilon_v-\epsilon},\qquad\epsilon\leq\epsilon_v.}
$$

Each [density of states](../../../../../density-of-states.md) is zero beyond its indicated band edge. The factor two counts spin; an extra valley degeneracy was not assumed in these stipulated isotropic bands.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
