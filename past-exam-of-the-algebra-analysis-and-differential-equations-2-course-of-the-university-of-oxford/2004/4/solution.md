<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the boundary form of [Cauchy's integral theorem](../../../cauchy-s-integral-theorem.md): the integral of a [holomorphic function](../../../holomorphic-function-split.md) around the oriented boundary of a compact region on whose neighborhood it is [holomorphic](../../../holomorphic-function-split.md) is zero, including annular regions with the inner boundary oppositely oriented. Apply it to $f(z)/(z-a)$ between the circles of radii $r$ and $\rho$, both around $a$. It gives

$$
\frac1{2\pi i}\int_{|z-a|=r}\frac{f(z)}{z-a}\,dz
=\frac1{2\pi}\int_0^{2\pi}f(a+\rho e^{it})\,dt\longrightarrow f(a)
$$

as $\rho\downarrow0$, by continuity. This proves the [Cauchy integral formula](../../../cauchy-integral-formula.md).

For a bounded [entire function](../../../entire-function.md) with $|f|\le M$, apply that formula at variable points inside a fixed circle and differentiate its kernel under the integral. At its center $a$, this gives

$$
f'(a)=\frac1{2\pi i}\int_{|z-a|=R}\frac{f(z)}{(z-a)^2}\,dz,
\qquad |f'(a)|\le\frac MR.
$$

The circle can have any radius because the function is entire. Letting $R\to\infty$ gives $f'(a)=0$ at every $a$, so $f$ is constant. This proves [Liouville's theorem](../../../liouville-theorem.md).

Finally, if a nonconstant [entire function](../../../entire-function.md) omitted all points within distance $\epsilon$ of some $w$, then $g=1/(f-w)$ would be entire and bounded by $1/\epsilon$. [Liouville's theorem](../../../liouville-theorem.md) would make $g$, and hence $f$, constant. Therefore every such neighborhood contains a value of $f$, proving the [dense image of a nonconstant entire function](../../../dense-image-of-a-nonconstant-entire-function.md) property.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2004](../../2004-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
