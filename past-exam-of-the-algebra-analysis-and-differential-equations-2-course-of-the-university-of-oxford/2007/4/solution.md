<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the following boundary version of [Cauchy's integral theorem](../../../cauchy-s-integral-theorem.md): if a function is [holomorphic](../../../holomorphic-function-split.md) on a neighborhood of a compact region bounded by finitely many piecewise smooth simple closed curves, its integral around the positively oriented boundary is zero. On an [annulus](../../../annulus-mathematics.md) this means that its integrals around the two circles, both taken counterclockwise, are equal.

For $0<\rho<r$, the function $f(z)/(z-w)$ is [holomorphic](../../../holomorphic-function-split.md) on a neighborhood of $\rho\le|z-w|\le r$. The theorem therefore gives

$$
\frac1{2\pi i}\int_{|z-w|=r}\frac{f(z)}{z-w}\,dz
=\frac1{2\pi}\int_0^{2\pi}f(w+\rho e^{it})\,dt.
$$

As $\rho\downarrow0$, continuity of $f$ makes the integrand converge uniformly to $f(w)$. The right side tends to $f(w)$, proving [Cauchy integral formula](../../../cauchy-integral-formula.md) without assuming that formula in an intermediate step.

Let $I$ denote the requested boundary integral. Parametrize the [unit circle](../../../complex-unit-circle.md) by $z=e^{it}$. Since $dz=ie^{it}dt$,

$$
I=\frac1{2\pi}\int_0^{2\pi}
\frac{\overline{f(e^{it})}}{1-ae^{-it}}\,dt.
$$

Taking [complex conjugates](../../../complex-conjugate.md) and using $\overline{e^{it}}=e^{-it}$ gives

$$
\overline I=\frac1{2\pi}\int_0^{2\pi}
\frac{f(e^{it})}{1-\overline a e^{it}}\,dt
=\frac1{2\pi i}\int_{|z|=1}\frac{f(z)}{z(1-\overline a z)}\,dz.
$$

This is the [conjugated Cauchy integral on a circle](../../../conjugated-cauchy-integral-on-a-circle.md) identity. The function $h(z)=f(z)/(1-\overline a z)$ is [holomorphic](../../../holomorphic-function-split.md) on a neighborhood of the closed [unit disc](../../../unit-disc.md), because $|a|<1$. Applying [Cauchy integral formula](../../../cauchy-integral-formula.md) at zero gives $\overline I=h(0)=f(0)$. Thus

$$
\boxed{I=\overline{f(0)}.}
$$

The [complex conjugates](../../../complex-conjugate.md) in these formulas are essential; the boundary integrand contains $\overline{f(z)}$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
