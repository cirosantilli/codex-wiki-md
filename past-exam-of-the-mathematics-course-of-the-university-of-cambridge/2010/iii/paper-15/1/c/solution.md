<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using the coordinate formula for the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md), the two components are

$$
[X,Y]^x=X(0)-Y(y)=-\frac{x^2}{2},\qquad
[X,Y]^y=X(x^2/2)-Y(0)=xy.
$$

Thus $\boxed{[X,Y]=-(x^2/2)\partial_x+xy\partial_y}$, which is not the zero [vector field](../../../../../../vector-field.md).

The [integral curves of a vector field](../../../../../../integral-curve-of-a-vector-field.md) $X$ solve $\dot x=y$, $\dot y=0$, whereas those of $Y$ solve $\dot x=0$, $\dot y=x^2/2$. Their [local flows](../../../../../../local-flow.md) are

$$
\boxed{\phi_t(x,y)=(x+ty,y),\qquad \psi_s(x,y)=(x,y+sx^2/2).}
$$

Both formulas exist for all real parameters, so both are [complete vector fields](../../../../../../complete-vector-field.md). Direct composition gives

$$
\phi_t\psi_s(x,y)=(x+ty+tsx^2/2,\ y+sx^2/2),\qquad
\psi_s\phi_t(x,y)=(x+ty,\ y+s(x+ty)^2/2).
$$

At $(1,0)$ their first coordinates differ by $ts/2$. Hence these [local flows](../../../../../../local-flow.md) do not commute when $s,t$ are nonzero.

For the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md), start at $(2,0)$. An [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md) $[X,Y]$ is

$$
(x(t),y(t))=\left(\frac{2}{1+t},0\right),\qquad -1<t<\infty.
$$

It solves $\dot x=-x^2/2$, $\dot y=xy$, but $x(t)$ diverges as $t\downarrow-1$. It cannot extend through that finite time as a curve in $\mathbb R^2$. **Complete vector fields are therefore not closed under the Lie bracket.**

For the sum $X+Y$, its [integral curves of a vector field](../../../../../../integral-curve-of-a-vector-field.md) obey $\dot x=y$, $\dot y=x^2/2$. Substitution of $x=(1+\alpha t)^{-2}$ and $y=\beta(1+\alpha t)^{-3}$ requires

$$
\beta=-2\alpha,\qquad -3\alpha\beta=\frac12,
\qquad \alpha^2=\frac1{12}.
$$

Choosing $\alpha=-1/(2\sqrt3)$ gives the [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md)

$$
\gamma(t)=\left(\left(1-\frac{t}{2\sqrt3}\right)^{-2},
\frac1{\sqrt3}\left(1-\frac{t}{2\sqrt3}\right)^{-3}\right),\qquad t<2\sqrt3.
$$

It starts at $(1,1/\sqrt3)$ and escapes to infinity at the finite time $2\sqrt3$. **Complete vector fields are not closed under addition either.** Both failures use the same pair of [complete vector fields](../../../../../../complete-vector-field.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
