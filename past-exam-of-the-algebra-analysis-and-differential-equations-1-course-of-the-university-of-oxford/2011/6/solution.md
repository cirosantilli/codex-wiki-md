<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [contour integral](../../../contour-integral.md) along a piecewise smooth path is defined by parametrization:

$$
\int_\gamma f(z)\,dz=\int_a^b f(\gamma(t))\gamma'(t)\,dt,
$$

with a sum over the smooth pieces. The [residue theorem](../../../residue-theorem.md) states that for a positively oriented simple closed contour and a function holomorphic on and inside it apart from finitely many isolated singularities $a_j$ inside,

$$
\oint_\gamma f(z)\,dz=2\pi i\sum_j\operatorname{Res}(f,a_j).
$$

More generally a closed contour uses the [winding number](../../../winding-number.md) of each singularity as its weight.

Set $z=e^{it}$, so $dt=dz/(iz)$ and $\cos t=(z+z^{-1})/2$. The required real [integral](../../../integral-split.md) becomes

$$
I=\frac1i\oint_{|z|=1}\frac{z}{2z^4+5z^2+2}\,dz.
$$

The denominator factors as $(2z^2+1)(z^2+2)$. Only the simple [poles](../../../pole.md) $z=\pm i/\sqrt2$ lie inside the [unit circle](../../../complex-unit-circle.md). At either one,

$$
\operatorname{Res}\left(\frac z{2z^4+5z^2+2},z_0\right)
=\frac{z_0}{8z_0^3+10z_0}=\frac1{8z_0^2+10}=\frac16.
$$

The [residue theorem](../../../residue-theorem.md) now gives

$$
\boxed{I=\frac1i\,2\pi i\left(\frac16+\frac16\right)=\frac{2\pi}{3}.}
$$

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2011](../../2011-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
