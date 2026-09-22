<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

The [chain rule](../../../../../chain-rule.md) for [Fréchet derivatives](../../../../../frechet-derivative.md) states that if $f$ is [differentiable](../../../../../differentiable-function.md) at $a$ and $g$ is [differentiable](../../../../../differentiable-function.md) at $f(a)$, then

$$
\boxed{D(g\circ f)_a=Dg_{f(a)}\circ Df_a}.
$$

The composition on the right is a composition of [linear maps](../../../../../linear-map.md), equivalently a product of [Jacobian matrices](../../../../../jacobian-matrix.md) in coordinates.

Apply the [chain rule](../../../../../chain-rule.md) to the [affine function](../../../../../affine-function.md) $x\mapsto(x,c-x)$. The resulting [derivative](../../../../../derivative.md) is

$$
\boxed{g_c'(x)=f_x(x,c-x)-f_y(x,c-x)}.
$$

If the two [partial derivatives](../../../../../partial-derivative.md) agree everywhere, $g_c'=0$. The [mean value theorem](../../../../../mean-value-theorem.md) makes $g_c$ constant on $\mathbb R$. Define $h(c)=f(c,0)$, which is itself [differentiable](../../../../../differentiable-function.md) by the [chain rule](../../../../../chain-rule.md). Taking $c=x+y$ gives $g_c(x)=g_c(c)=h(c)$, and therefore

$$
\boxed{f(x,y)=h(x+y)}.
$$

No [continuity](../../../../../continuous-function.md) of the [partial derivatives](../../../../../partial-derivative.md) beyond the assumed [differentiability](../../../../../differentiability.md) is needed.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
