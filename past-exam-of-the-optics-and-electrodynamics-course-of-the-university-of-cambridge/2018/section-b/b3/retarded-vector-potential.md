<h1 id="section-b/b3/retarded-vector-potential">Retarded vector potential</h1>

↑ **Parent:** [Solution](solution.md)

For a localized [current density](../../../../current-density.md), the retarded [magnetic vector potential](../../../../magnetic-vector-potential.md) is

$$
\mathbf A(\mathbf r,t)=\frac{\mu_0}{4\pi}\int
\frac{\mathbf J(\mathbf r',t-|\mathbf r-\mathbf r'|/c)}{|\mathbf r-\mathbf r'|}\,d^3r'.
$$

At large $r$, replace the amplitude denominator by $r$. For an electrically short dipole, the delay difference across its length is negligible compared with an oscillation period, so evaluate all currents at $t_r=t-r/c$. The [continuity equation for electric charge](../../../../charge-continuity-equation.md) gives the identity

$$
\dot{\mathbf p}(t)=\frac{d}{dt}\int\mathbf r'\rho(\mathbf r',t)\,d^3r'
=-\int\mathbf r'\nabla'\cdot\mathbf J\,d^3r'
=\int\mathbf J\,d^3r',
$$

where localization makes the boundary term vanish. Hence

$$
\boxed{\mathbf A(\mathbf r,t)\simeq\frac{\mu_0}{4\pi r}\dot{\mathbf p}(t-r/c)
=-\frac{\mu_0\omega p_0}{4\pi r}\sin[\omega(t-r/c)]\widehat{\mathbf z}.}
$$

In this gauge its Cartesian direction is fixed and its magnitude depends only on $r$ and the retarded dipole motion, with $1/r$ spreading. Spherical components have the geometric factors $\cos\theta$ and $-\sin\theta$ above; the angular radiation pattern arises after differentiating the potentials, not from an isotropic radiated intensity.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B3](../b3.md)
3. [Section B](../../section-b.md)
4. [2018](../../../2018-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
