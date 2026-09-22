<h1 id="analysis/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose a small positively oriented circle $C_\varepsilon$ about $z_0$ inside the given region. Cauchy's theorem on the region between the two [contours](../../../../complex-integration-contour.md) gives

$$
\int_\gamma\frac{f(z)}{z-z_0}\,dz=\int_{C_\varepsilon}\frac{f(z)}{z-z_0}\,dz=i\int_0^{2\pi}f(z_0+\varepsilon e^{it})\,dt.
$$

[Continuity](../../../../continuous-function.md) makes the last integrand converge uniformly to $f(z_0)$ as $\varepsilon\downarrow0$. Its limit is $2\pi if(z_0)$, proving the [Cauchy integral formula](../../../../cauchy-integral-formula.md).

The same formula holds with an interior point $w$ near $z_0$. Subtract its value at $z_0$ and divide by $w-z_0$:

$$
\frac{f(w)-f(z_0)}{w-z_0}=\frac1{2\pi i}\int_\gamma\frac{f(z)}{(z-w)(z-z_0)}\,dz.
$$

The [contour](../../../../complex-integration-contour.md) is a positive distance from $z_0$, so the integrands converge uniformly as $w\to z_0$. Passing to the limit gives the differentiated formula

$$
\boxed{f'(z_0)=\frac1{2\pi i}\int_\gamma\frac{f(z)}{(z-z_0)^2}\,dz.}
$$

On the [unit circle](../../../../complex-unit-circle.md), $\bar z=1/z$ and $\operatorname{Im}z=(z-\bar z)/(2i)$, proving the requested identity. Hence the requested integral is

$$
\frac1{2i}\left[\int_{|z|=1}\frac{dz}{3z-1}-\int_{|z|=1}\frac{dz}{z^2(3z-1)}\right].
$$

The first integral is $2\pi i/3$. For the second use

$$
\frac1{z^2(3z-1)}=-\frac1{z^2}-\frac3z+\frac9{3z-1}.
$$

The differentiated formula applied to the constant function gives $\int z^{-2}\,dz=0$; the remaining two terms integrate to $-6\pi i+6\pi i=0$. Therefore

$$
\boxed{\int_{|z|=1}\frac{\operatorname{Im}z}{z(3z-1)}\,dz=\frac\pi3.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Analysis](../../analysis.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
