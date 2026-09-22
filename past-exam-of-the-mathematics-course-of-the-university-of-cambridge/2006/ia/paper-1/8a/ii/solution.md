<h1 id="8a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the given [Möbius transformation](../../../../../../mobius-transformation.md), the [fixed point](../../../../../../fixed-point.md) equation is $z(z+3)=3z+1$, hence

$$
\boxed{z=1,\qquad z=-1.}
$$

For the general [Möbius transformation](../../../../../../mobius-transformation.md), its finite fixed points satisfy

$$
cz^2+(d-a)z-b=0.
$$

With $c\ne0$ and nonzero [discriminant](../../../../../../discriminant.md), the [quadratic formula](../../../../../../quadratic-formula.md) gives the two distinct [fixed points of a Möbius transformation](../../../../../../fixed-point-of-a-mobius-transformation.md):

$$
\boxed{\alpha=\frac{a-d+m}{2c},\qquad\beta=\frac{a-d-m}{2c},\qquad m^2=(a-d)^2+4bc.}
$$

The fixed-point equation for $\alpha$ also gives $b-d\alpha=-\alpha(a-c\alpha)$. Therefore

$$
\omega-\alpha=\frac{(a-c\alpha)(z-\alpha)}{cz+d},
\qquad
\omega-\beta=\frac{(a-c\beta)(z-\beta)}{cz+d}.
$$

Dividing yields the [conjugation of a Möbius transformation with two distinct fixed points](../../../../../../conjugation-of-a-mobius-transformation-with-two-distinct-fixed-points.md):

$$
\boxed{\frac{\omega-\alpha}{\omega-\beta}
=k\frac{z-\alpha}{z-\beta},\qquad
k=\frac{a-c\alpha}{a-c\beta}=\frac{a+d-m}{a+d+m}.}
$$

Neither factor in this quotient vanishes, since $(a-c\alpha)(a-c\beta)=ad-bc\ne0$. The formula extends over the [Riemann sphere](../../../../../../riemann-sphere.md), including the transformation's pole. For the special transformation and the ordering $\alpha=1,\beta=-1$, $k=1/2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8A](../../8a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
