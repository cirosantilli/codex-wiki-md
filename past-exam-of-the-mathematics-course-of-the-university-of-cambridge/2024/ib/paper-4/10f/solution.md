<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Differentiability at $x\in\mathbb R^2$ means that there is a [linear map](../../../../../linear-map.md) $Df|_x:\mathbb R^2\to\mathbb R$ such that

$$
f(x+h)=f(x)+Df|_x(h)+o(\|h\|).
$$

The [partial derivatives](../../../../../partial-derivative.md) are $D_if(x)=Df|_x(e_i)$ when the [derivative](../../../../../derivative.md) exists; independently, they may be defined by the corresponding one-variable difference quotients.

Suppose the [partial derivatives](../../../../../partial-derivative.md) exist near $x=(x_1,x_2)$ and are continuous at $x$. Apply the one-dimensional mean value theorem along the two coordinate segments from $x$ to $x+h$. It gives intermediate points $\xi_h,\eta_h\to x$ such that

$$
f(x+h)-f(x)
=D_1f(\xi_h)h_1+D_2f(\eta_h)h_2.
$$

Continuity of the partials makes the remainder after subtracting

$$
D_1f(x)h_1+D_2f(x)h_2
$$

equal to $o(\|h\|)$. Hence $f$ is [differentiable](../../../../../differentiable-function.md) and this is its [derivative](../../../../../derivative.md).

For the given [function](../../../../../function-split.md), writing $r=\sqrt{x^2+y^2}$, at $r>0$ we have

$$
\boxed{
D_1f=2x\sin(1/r)-\frac{x}{r}\cos(1/r),
\qquad
D_2f=2y\sin(1/r)-\frac{y}{r}\cos(1/r)}.
$$

At the origin both [partial derivatives](../../../../../partial-derivative.md) are zero, since $f(h,0)/h$ and $f(0,h)/h$ tend to zero. Neither partial is continuous there: along its corresponding coordinate axis the cosine term oscillates without a [limit](../../../../../limit-of-a-function.md). Nevertheless

$$
|f(x,y)|\leq r^2=o(r),
$$

so $f$ is [differentiable](../../../../../differentiable-function.md) at the origin with [derivative](../../../../../derivative.md) zero. This illustrates that [existence of partial derivatives does not imply their continuity](../../../../../existence-of-partial-derivatives-does-not-imply-their-continuity.md).

The final assertion is false. Define

$$
g(x,y)=
\begin{cases}
(x^2+y^2)\sin\!\left(\dfrac1{x^2+y^2}\right),&(x,y)\ne(0,0),\\
0,&(x,y)=(0,0).
\end{cases}
$$

Again $|g|\leq r^2$, so $g$ is [differentiable](../../../../../differentiable-function.md) at the origin and it is smooth elsewhere. But along the $x$-axis,

$$
D_1g(x,0)=2x\sin(1/x^2)-\frac2x\cos(1/x^2),
$$

is unbounded near zero, and similarly $D_2g(0,y)$ is unbounded. Thus both [partial derivatives](../../../../../partial-derivative.md) can be unbounded in every neighbourhood of a point even when the [function](../../../../../function-split.md) is [differentiable](../../../../../differentiable-function.md) everywhere.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
