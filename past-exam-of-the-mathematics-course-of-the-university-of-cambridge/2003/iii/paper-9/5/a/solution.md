<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We prove necessity of the geometric condition from the embedding condition. Use normalized angular measure $m$ and the [H1 space on the unit disk](../../../../../../h1-space-on-the-unit-disk.md) norm $\|f\|_1=\sup_{r<1}\int|f(r\xi)|\,dm(\xi)$. Testing $f=1$ first gives $\mu(\mathbb D)\le N(\mu)$.

For a short arc $I$ of normalized length $\ell=m(I)$ centered at $\xi_0$, put $a=(1-\ell)\xi_0$ and use the [normalized squared Cauchy kernel](../../../../../../normalized-squared-cauchy-kernel.md)

$$
f_a(z)=\frac{1-|a|^2}{(1-\overline a z)^2}.
$$

Its boundary modulus is the [Poisson kernel on the circle](../../../../../../poisson-kernel-on-the-circle.md), so $\|f_a\|_1=1$. The [geodesic-cap and Carleson-box comparison](../../../../../../geodesic-cap-and-carleson-box-comparison.md) gives $|z-\xi_0|\le C\ell$ for $z\in Q(I)$. Therefore $|1-\overline a z|\le C'\ell$, whereas $1-|a|^2=2\ell-\ell^2\ge\ell$. Thus $|f_a(z)|\ge c/\ell$ throughout the [hyperbolic geodesic cap](../../../../../../hyperbolic-geodesic-cap.md). The embedding bound gives

$$
\frac c\ell\mu(Q(I))\le\int_{\mathbb D}|f_a|\,d\mu\le N(\mu).
$$

For arcs longer than a fixed small threshold, the total-mass estimate gives the same form after changing the absolute constant. Hence

$$
\boxed{\mu(Q(I))\le C N(\mu)m(I).}
$$

This is precisely the [Carleson measure](../../../../../../carleson-measure.md) condition, in its geodesic-cap version.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
