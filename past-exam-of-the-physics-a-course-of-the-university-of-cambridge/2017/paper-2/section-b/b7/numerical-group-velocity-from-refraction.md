<h1 id="section-b/b7/numerical-group-velocity-from-refraction">Numerical group velocity from refraction</h1>

↑ **Parent:** [Solution](solution.md)

The wavelengths specified for incidence from vacuum are $\lambda_0$. With fixed incident angle $\theta_i$, [Snell's law](../../../../../snell-s-law.md) gives $n=\sin\theta_i/\sin\theta_t$ and $v_p=c\sin\theta_t/\sin\theta_i$. At the central wavelength,

$$
n=\frac{\sin45.00^\circ}{\sin17.80^\circ}=2.3131,\qquad
v_p=1.2961\times10^8\,\mathrm{m\,s^{-1}}.
$$

Use a central difference, converting the angle change to radians:

$$
\frac{d\theta_t}{d\lambda_0}\simeq\frac{0.020\pi/180}{4.0\times10^{-9}}
=8.7266\times10^4\,\mathrm{rad\,m^{-1}}.
$$

The [group index from refracted-angle dispersion](../../../../../group-index-from-refracted-angle-dispersion.md) is

$$
n_g=n\left[1+\lambda_0\cot\theta_t\frac{d\theta_t}{d\lambda_0}\right]=2.6275,
\qquad
\boxed{v_g=\frac c{n_g}=1.141\times10^8\,\mathrm{m\,s^{-1}}}.
$$

Directly inserting the incident vacuum wavelengths into $v_p-\lambda\,dv_p/d\lambda$ would instead give $1.120\times10^8\,\mathrm{m\,s^{-1}}$. That is a plausible intended rough answer, but it mixes wavelength coordinates; the boxed result consistently uses the incident data. The two agree only to first order in a sufficiently small dimensionless dispersion correction.

## ↑ Ancestors (15)

1. [Solution](solution.md)
2. [B7](../b7.md)
3. [Section B](../../section-b.md)
4. [Paper 2](../../../paper-2-split.md)
5. [2017](../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
