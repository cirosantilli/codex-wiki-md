<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mu=GM$ and $s=\sqrt{b^2+r^2}$. The [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) of the [spherical isochrone model](../../../../../../spherical-isochrone-model.md) obeys

$$
\frac{d\Phi}{dr}=\frac{\mu r}{s(b+s)^2}.
$$

The spherical [Poisson equation](../../../../../../poisson-equation.md) therefore gives

$$
\begin{aligned}
\rho(r)
&=\frac1{4\pi Gr^2}\frac d{dr}
\left(r^2\frac{d\Phi}{dr}\right)\\
&=\frac{M}{4\pi s(b+s)^2}
\left(3-\frac{r^2}{s^2}
-\frac{2r^2}{s(b+s)}\right).
\end{aligned}
$$

Its small-radius [asymptotic expansion](../../../../../../asymptotic-expansion.md) is

$$
\boxed{
\rho(r)=\frac{3M}{16\pi b^3}
-\frac{5Mr^2}{16\pi b^5}+O(r^4)},
\qquad r\ll b,
$$

so the model has a finite-density core. At large radius,

$$
\boxed{
\rho(r)=\frac{Mb}{2\pi r^4}
-\frac{3Mb^2}{4\pi r^5}+O(r^{-6})},
\qquad r\gg b.
$$

The $r^{-4}$ envelope has finite total mass $M$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
