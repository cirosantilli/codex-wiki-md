<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $h(x,y)=\tfrac12\log(x^2+y^2)$ away from the origin,

$$
\nabla h=\frac{(x,y)}{x^2+y^2},\quad h_{xx}=\frac{y^2-x^2}{(x^2+y^2)^2},\quad h_{yy}=\frac{x^2-y^2}{(x^2+y^2)^2},\quad\Delta h=0.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) for [planar Brownian motion](../../../../../../planar-brownian-motion.md) therefore has no drift term before the radius reaches $r$. Since the initial logarithm is zero,

$$
\boxed{\log|B_{t\wedge S_r}|=\int_0^{t\wedge S_r}\frac{B_s^1\,dB_s^1+B_s^2\,dB_s^2}{|B_s|^2}.}
$$

The integrand's squared norm is $|B_s|^{-2}\leq r^{-2}$ on this stopped interval, so this is a square-integrable [martingale](../../../../../../martingale-split.md) on every finite horizon, in particular a [local martingale](../../../../../../local-martingale.md). One may first stop in an outer annulus to apply the formula on a compact smooth domain and then remove that localization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
