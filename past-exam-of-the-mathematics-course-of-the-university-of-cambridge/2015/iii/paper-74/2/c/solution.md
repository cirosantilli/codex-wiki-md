<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the [gravity current](../../../../../../gravity-current.md) nose, the depth and [velocity](../../../../../../velocity.md) change over a distance comparable with the depth, with appreciable vertical acceleration and mixing. The [hydrostatic approximation](../../../../../../hydrostatic-approximation.md) and the depth-uniform interior model do not resolve that structure. A suitable [gravity-current front condition](../../../../../../gravity-current-front-condition.md) is

$$
\boxed{\dot X=\operatorname{Fr}\sqrt{G\phi h},}
$$

with a positive, order-one [Froude number](../../../../../../froude-number.md) determined by the nose closure and geometry. It is not fixed by the interior equations alone. This definition uses $\sqrt{g'h}$; if the front condition is expressed using $c=\sqrt{g'h/2}$, its numerical coefficient changes by $\sqrt2$.

For a late-time [gravity-current box model](../../../../../../gravity-current-box-model.md), take the depth and [particle volume fraction](../../../../../../particle-volume-fraction.md) to be uniform over $0<x<X(t)$, and neglect entrainment and resuspension. The initial [volume](../../../../../../volume.md) is $\mathcal V=\beta h_0^2L/2$, so

$$
\frac{\beta h^2X}{2}=\mathcal V,\qquad h=h_0\sqrt{\frac LX}.
$$

The total particle [volume](../../../../../../volume.md) is $\mathcal V\phi$. Deposition over the projected boundary width gives $d(\mathcal V\phi)/dt=-\beta hXw\phi$. With the specified [hindered settling](../../../../../../hindered-settling.md) factor, the [prismatic triangular-channel gravity-current box model](../../../../../../prismatic-triangular-channel-gravity-current-box-model.md) is

$$
\boxed{\dot X=\operatorname{Fr}\sqrt{G\phi h},\qquad
\dot\phi=-\frac{2w_0}{h}\phi(1-\phi),\qquad h=h_0\sqrt{L/X}.}
$$

Initializing this approximate model with $X(0)=L$ and $\phi(0)=\phi_0$ matches the original [volume](../../../../../../volume.md) and [concentration](../../../../../../concentration.md); it does not assert that the immediate dam-break flow is a uniform box.

Eliminate time to obtain

$$
\frac{d\phi}{\sqrt\phi(1-\phi)}=-\frac{2w_0X^{3/4}}{\operatorname{Fr}\sqrt G\,h_0^{3/2}L^{3/4}}\,dX.
$$

Since the left primitive is $2\operatorname{artanh}\sqrt\phi$, the [hindered-settling runout invariant in a prismatic triangular channel](../../../../../../hindered-settling-runout-invariant-in-a-prismatic-triangular-channel.md) is

$$
\boxed{\operatorname{artanh}\sqrt\phi
=\operatorname{artanh}\sqrt{\phi_0}-\frac{4w_0}{7\operatorname{Fr}\sqrt G\,h_0^{3/2}L^{3/4}}(X^{7/4}-L^{7/4}).}
$$

This relation, the [volume](../../../../../../volume.md) constraint and $\dot X$ determine the late-time evolution. If desired, the time is given by the quadrature $t=\int_L^{X(t)}[\operatorname{Fr}\sqrt{G\phi(s)h_0\sqrt{L/s}}]^{-1}\,ds$. The physical branch has nonnegative right-hand side in the boxed relation; it ends when that expression reaches zero.

Thus the limiting [runout length of a gravity current](../../../../../../runout-length-of-a-gravity-current.md), measured from the closed end, is

$$
\boxed{X_\infty=\left[L^{7/4}+\frac{7\operatorname{Fr}\sqrt G\,h_0^{3/2}L^{3/4}}{4w_0}\operatorname{artanh}\sqrt{\phi_0}\right]^{4/7}.}
$$

The advance beyond the dam is $X_\infty-L$. In the dilute limit, $\operatorname{artanh}\sqrt{\phi_0}\simeq\sqrt{\phi_0}$. The ideal model approaches its finite [runout length of a gravity current](../../../../../../runout-length-of-a-gravity-current.md) only as $t\to\infty$: near the limit $\phi$ decays exponentially with rate $2w_0/h_\infty$ and the front speed tends to zero. The exponent $7/4$ uses the prismatic triangular geometry; a channel widening with $x$ has a different [volume](../../../../../../volume.md) constraint and runout law.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
