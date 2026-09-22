<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Differentiability means existence of a [linear map](../../../../../linear-map.md) $A:\mathbb R^2\to\mathbb R$ such that

$$
f(x_0+h,y_0+k)=f(x_0,y_0)+A(h,k)+r(h,k),\qquad\frac{r(h,k)}{\sqrt{h^2+k^2}}\longrightarrow0.
$$

This is the [Fréchet derivative](../../../../../frechet-derivative.md). Substituting increments on the coordinate axes shows $A(h,k)=f_x(x_0,y_0)h+f_y(x_0,y_0)k$. For the unit direction $v=(\cos\alpha,\sin\alpha)$, the remainder is $r(tv)=o(|t|)$. Dividing the increment by $t$ proves differentiability of the restricted function and gives its [directional derivative](../../../../../directional-derivative.md):

$$
\boxed{g_\alpha'(0)=f_x(x_0,y_0)\cos\alpha+f_y(x_0,y_0)\sin\alpha.}
$$

For the supplied rational function, both coordinate-axis restrictions are zero, so $f_x(0,0)=f_y(0,0)=0$. Any [Fréchet derivative](../../../../../frechet-derivative.md) would therefore be the zero map. But $f(t,t)=t$, and hence $|f(t,t)|/\sqrt{t^2+t^2}=1/\sqrt2$ for nonzero $t$. This contradicts the required vanishing remainder. Thus

$$
\boxed{f\text{ is not differentiable at }(0,0).}
$$

In fact every [directional derivative](../../../../../directional-derivative.md) exists: along $v$ it equals $\cos^2\alpha\sin\alpha+\cos\alpha\sin^2\alpha$. These values do not depend linearly on the direction, illustrating why existence of directional derivatives is weaker than differentiability.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
