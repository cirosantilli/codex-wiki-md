<h1 id="section-a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose a coordinate $z$ measured from the sphere centre towards increasing distance from the block, so an atom in the sphere is at height $L+z$. Summing the atom–block [potential energy](../../../../potential-energy.md) with the sphere's [number density](../../../../number-density.md) gives

$$
U(L)=-\frac{B\pi n^2}{6}\int_{|\boldsymbol x|<R}\frac{d^3x}{(L+z)^3}.
$$

For $R/L\ll1$, a uniformly valid [Taylor series](../../../../taylor-series.md) over the sphere is

$$
\frac1{(L+z)^3}=\frac1{L^3}\left[1-\frac{3z}{L}+\frac{6z^2}{L^2}-\frac{10z^3}{L^3}+O\!\left(\frac{z^4}{L^4}\right)\right].
$$

The odd moments vanish by reflection symmetry. The sphere volume is $V_s=4\pi R^3/3$, and its second moment is

$$
\int z^2d^3x=\pi\int_{-R}^{R}z^2(R^2-z^2)dz=\frac{4\pi R^5}{15}=\frac{V_sR^2}{5}.
$$

Consequently

$$
\boxed{U(L)=-\frac{2\pi^2Bn^2R^3}{9L^3}
\left[1+\frac65\frac{R^2}{L^2}+O\!\left(\frac{R^4}{L^4}\right)\right].}
$$

The first finite-radius correction is therefore $-4\pi^2Bn^2R^5/(15L^5)$. There is no relative $R/L$ correction because the first moment about the centre is zero. The leading term is just the number of sphere atoms times the potential at its centre; the correction increases the attraction because the nearer atoms contribute more strongly than the farther atoms lose.

This is the [far-field sphere-plane dispersion energy](../../../../far-field-sphere-plane-dispersion-energy.md), with [Hamaker constant](../../../../hamaker-constant.md) $A_H=\pi^2Bn^2$. It must be distinguished from the near-contact [sphere-plane dispersion force](../../../../sphere-plane-dispersion-force.md), whose small parameter is the surface gap divided by the radius. Here $L$ is explicitly the centre-to-plane distance.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
