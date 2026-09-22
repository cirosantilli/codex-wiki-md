<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The centrifugal criterion concerns axisymmetric disturbances, so set $m=0$. The azimuthal equation gives

$$
v'=-\frac{2\Omega+r\Omega'}{\sigma}u'.
$$

Eliminating $w'$ with incompressibility and then $p'$ with the axial equation yields

$$
\boxed{
\frac d{dr}\left[\frac1r\frac d{dr}(ru')\right]
-k^2\left(1+\frac{\Phi(r)}{\sigma^2}\right)u'=0},
$$

where the [Rayleigh discriminant](../../../../../../rayleigh-discriminant.md) is

$$
\boxed{
\Phi(r)=2\Omega(2\Omega+r\Omega')
=\frac1{r^3}\frac d{dr}(r^4\Omega^2)}.
$$

Impermeability at the two solid walls gives $u'(r_i)=u'(r_o)=0$.

Multiply the equation by $r\overline{u'}$, integrate between the walls, and use [integration by parts](../../../../../../integration-by-parts.md). The boundary terms vanish and one obtains

$$
\sigma^2
=-\frac{k^2\displaystyle\int_{r_i}^{r_o}
r\Phi|u'|^2\,dr}
{\displaystyle\int_{r_i}^{r_o}
\frac{|(ru')'|^2}{r}\,dr
+k^2\displaystyle\int_{r_i}^{r_o}r|u'|^2\,dr}.
$$

The denominator is positive. Therefore $\Phi\geq0$ throughout the annulus excludes positive real $\sigma^2$ and gives centrifugal stability. Since $r^4\Omega^2=(r^2\Omega)^2$ is the square of the [specific angular momentum](../../../../../../specific-angular-momentum.md), [Rayleigh's circulation criterion](../../../../../../rayleigh-s-circulation-criterion.md) is

$$
\boxed{
\frac d{dr}(r^2\Omega)^2\geq0
\quad\text{for centrifugal stability}}.
$$

An outward decrease of squared specific angular momentum permits an axisymmetric centrifugal instability.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
