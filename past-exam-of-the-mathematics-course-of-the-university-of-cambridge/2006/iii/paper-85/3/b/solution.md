<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\mu<0$, put $k=\sqrt{-\mu}$. There are no local [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) and $\dot x=x^2+k^2>0$, so every incoming point passes through the local region. The same sections give

$$
T_{\rm loc}(x)=\frac1k\left[\arctan\frac hk-\arctan\frac xk\right],\qquad
Y(x)=h\exp\left\{-\frac\lambda k\left[\arctan\frac hk-\arctan\frac xk\right]\right\},
$$

and again $P(x)=\nu+cY(x)+O(Y^2)$. The global return supplied by the problem closes the passage into a [periodic orbit](../../../../../../periodic-orbit.md) if this map has a [fixed point](../../../../../../fixed-point.md).

Its [derivative](../../../../../../derivative.md) is strongly contracting: $Y'(x)=\lambda Y(x)/(x^2+k^2)$. To see the smallness uniformly near the codimension-two point, put $d=\sqrt{x^2+k^2}$ and assume $2d<h$. The passage includes $[d,2d]$, on which $\xi^2+k^2\le5d^2$, so $T_{\rm loc}\ge1/(5d)$. Consequently

$$
|P'(x)|\le C\frac{e^{-\lambda/(5d)}}{d^2}\longrightarrow0\qquad(d\to0).
$$

For a sufficiently small entry interval and all sufficiently small $\nu$ of either sign, $P$ maps the interval into itself and has [derivative](../../../../../../derivative.md) bounded strictly below one. The [mean value theorem](../../../../../../mean-value-theorem.md) bounds differences by a factor strictly below one, while the endpoint signs of $P(x)-x$ give existence of a [fixed point](../../../../../../fixed-point.md). Thus

$$
\boxed{\text{a unique nearby attracting periodic orbit exists for }\mu<0\text{, for either sign of }\nu.}
$$

Here “all $\nu$” means all return parameters in the neighborhood where the stated local/global construction applies, not arbitrarily distant global return geometries.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
