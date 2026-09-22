<h1 id="14f/solution">Solution</h1>

↑ **Parent:** [14F](../14f.md)

Use the [conformal map of a vertical half-strip by sine](../../../../../conformal-map-of-a-vertical-half-strip-by-sine.md) followed by a [Cayley transform](../../../../../cayley-transform-hyperbolic-geometry.md):

$$
\boxed{F(z)=\frac{\sin z-i}{\sin z+i}.}
$$

We verify that this maps the entire half-strip bijectively onto the [unit disc](../../../../../unit-disc.md). First,

$$
\operatorname{Im}\sin(x+iy)=\cos x\sinh y>0,
$$

so the [sine](../../../../../sine.md) image lies in the upper half-plane. Also $\cos z\ne0$ in the domain, making the map locally a [conformal map](../../../../../conformal-map.md). If $\sin z=\sin w$, the identity for a difference of sines gives either $z-w=2\pi n$ or $z+w=(2n+1)\pi$. The real-part bounds force $n=0$ in the first case, while positive imaginary parts exclude the second. Thus [sine](../../../../../sine.md) is injective.

For surjectivity, given any $w$ in the upper half-plane, solve

$$
t^2-2iwt-1=0.
$$

No root is on the unit circle, since $w=(t-t^{-1})/(2i)$ would then be real. The product of the two roots is $-1$, so exactly one root has $|t|<1$. For this root,

$$
\operatorname{Im}w=\frac12\operatorname{Re}t\,(|t|^{-2}-1)>0,
$$

which forces $\operatorname{Re}t>0$. Choose its logarithm with argument in $(-\pi/2,\pi/2)$ and put $z=-i\log t$. Then $\operatorname{Im}z=-\log|t|>0$, its real part lies in the required interval, and $\sin z=w$. This proves that [sine](../../../../../sine.md) maps onto the upper half-plane.

Finally, for $\operatorname{Im}w>0$, $|w-i|<|w+i|$, and the [Möbius transformation](../../../../../mobius-transformation.md) $(w-i)/(w+i)$ is a bijection to the [unit disc](../../../../../unit-disc.md). Its inverse is $w=i(1+\zeta)/(1-\zeta)$. Both constituent derivatives are nonzero, completing the proof for the displayed [conformal map](../../../../../conformal-map.md).

## ↑ Ancestors (10)

1. [14F](../14f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
