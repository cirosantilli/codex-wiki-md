<h1 id="9c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Along the [holonomic constraint](../../../../../../holonomic-constraint.md) $z=x^2/(4a)$, we have $\dot z=x\dot x/(2a)$ and hence speed squared $(1+x^2/(4a^2))\dot x^2$. The smooth wire's [normal reaction](../../../../../../normal-force.md) is perpendicular to the permitted [velocity](../../../../../../velocity.md) and does no work. [Conservation of mechanical energy](../../../../../../conservation-of-mechanical-energy.md), with release from rest at height $h$, gives

$$
\frac12m\left(1+\frac{x^2}{4a^2}\right)\dot x^2+\frac{mgx^2}{4a}=mgh.
$$

The [turning points](../../../../../../turning-point.md) are $x=\pm x_0$ with $x_0=2\sqrt{ah}$. One full oscillation has twice the travel time between them:

$$
T=2\int_{-x_0}^{x_0}
\sqrt{\frac{1+x^2/(4a^2)}{2g[h-x^2/(4a)]}}dx.
$$

Set $x=x_0u$ and $\beta=h/a$. After cancelling the scale factors,

$$
T=2\sqrt{\frac{2a}{g}}\int_{-1}^1
\sqrt{\frac{1+\beta u^2}{1-u^2}}du,
$$

so the [bead on a parabolic wire](../../../../../../bead-on-a-parabolic-wire.md) has

$$
\boxed{G(\beta)=2\sqrt2\int_{-1}^1\sqrt{\frac{1+\beta u^2}{1-u^2}}du.}
$$

For $\beta\ll1$, expand the numerator uniformly on $[-1,1]$:

$$
\sqrt{1+\beta u^2}=1+\frac12\beta u^2+O(\beta^2).
$$

The integrable endpoint weight gives $\int_{-1}^1(1-u^2)^{-1/2}du=\pi$ and $\int_{-1}^1u^2(1-u^2)^{-1/2}du=\pi/2$, for example by $u=\sin\theta$. Therefore the requested small-oscillation period is

$$
\boxed{T=2\pi\sqrt{\frac{2a}{g}}
\left[1+\frac{h}{4a}+O\left((h/a)^2\right)\right].}
$$

The leading frequency is $\sqrt{g/(2a)}$, and the first finite-amplitude correction increases the period. At $h=0$ the ring is stationary; the expression is the limiting period of nonzero small oscillations.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9C](../../9c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
