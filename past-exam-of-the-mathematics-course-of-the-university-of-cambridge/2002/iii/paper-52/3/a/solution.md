<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\ell$ and $\mathcal T$ denote longitudinal length and time scales, and let $U$ be a typical streamwise [velocity](../../../../../../velocity.md). The [shallow water](../../../../../../shallow-water-approximation.md) approximation requires $h/\ell\ll1$, slow changes in the channel geometry $h|B'/B|\ll1$, and small longitudinal slopes. The vertical [velocity](../../../../../../velocity.md) is then of order $Uh/\ell$; its acceleration must be small compared with the restoring acceleration, for example $Uh/(\mathcal T\ell)+U^2h/\ell^2\ll g'$ in a reduced-gravity layer. The leading [pressure](../../../../../../pressure.md) is [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), and cross-sectional horizontal [velocity](../../../../../../velocity.md) is approximated by $u(x,t)$. High [Reynolds number](../../../../../../reynolds-number.md) permits negligible interior viscous terms but does not itself guarantee the geometric or hydrostatic assumptions. We also require $B>0$ and $h>0$ in the wetted interior. The dimensionless $B$ need not be small: it measures the cross-section's opening angle, while the smallness condition concerns streamwise variation.

The cross-sectional area and volume transport are

$$
A(x,t)=\int_0^h B(x)z\,dz=\frac{Bh^2}{2},\qquad q=Au.
$$

For an impermeable bed and no [fluid entrainment](../../../../../../fluid-entrainment.md), [volume conservation](../../../../../../volume-conservation.md) gives

$$
\boxed{\partial_t\left(\frac{Bh^2}{2}\right)+\partial_x\left(\frac{Bh^2u}{2}\right)=0,}
$$

or, equivalently,

$$
h_t+uh_x+\frac h2u_x=-\frac{uh}{2}\frac{B'}B.
$$

The geometrical source term expresses the depth change needed when a moving layer encounters a wider or narrower triangular section.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Section B](../../section-b.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
