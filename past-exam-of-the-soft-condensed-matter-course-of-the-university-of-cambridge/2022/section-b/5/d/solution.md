<h1 id="section-b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $k=\beta F$ and $q=k\delta$. The [absorbing boundary condition for a diffusion](../../../../../absorbing-boundary-condition-for-a-diffusion.md) gives $A=j_0e^q/(Dk)$, hence

$$
p(x)=\frac{j_0}{Dk}\left[e^{k(\delta-x)}-1\right].
$$

This is nonnegative throughout the allowed interval. Normalizing the [probability density](../../../../../probability-density.md) gives

$$
1=\frac{j_0}{Dk}\left[\frac{e^q-1}{k}-\delta\right]
=\frac{j_0}{Dk^2}(e^q-1-q).
$$

Therefore

$$
\boxed{j_0=\frac{D\beta^2F^2}{e^{\beta F\delta}-\beta F\delta-1},\qquad
A=\frac{\beta F\,e^{\beta F\delta}}{e^{\beta F\delta}-\beta F\delta-1}.}
$$

Equivalently the normalized density is

$$
p(x)=\frac{k[e^{k(\delta-x)}-1]}{e^q-1-q}.
$$

The denominator is positive for $q>0$, since $e^q>1+q$. The dimensions are consistent: $j_0$ has units of inverse time, $A$ and $p$ of inverse length, and $q$ is dimensionless.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
