<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $r>0$, the [partial derivatives](../../../../../../partial-derivative.md) $r_x=x/r$ and $r_y=y/r$ give

$$
\frac{\partial}{\partial x}\frac{x^2}{r}=\frac{2x}{r}-\frac{x^3}{r^3},\qquad
\frac{\partial}{\partial y}\frac{xy}{r}=\frac{x}{r}-\frac{xy^2}{r^3}.
$$

Adding these [partial derivatives](../../../../../../partial-derivative.md) yields the [divergence](../../../../../../divergence.md):

$$
\boxed{\nabla\cdot\mathbf f=\frac{3x}{r}-\frac{x(x^2+y^2)}{r^3}=\frac{2x}{\sqrt{x^2+y^2}},\qquad (x,y)\ne(0,0).}
$$

The original [vector field](../../../../../../vector-field.md) is undefined at the origin. Since $\|\mathbf f\|=|x|\leq r$, it has the [continuous extension](../../../../../../continuous-extension.md) $\mathbf f(0,0)=\mathbf0$. This extension is not [differentiable](../../../../../../differentiable-function.md): on $y=0$ its first component is $|x|$, whose [derivative](../../../../../../derivative.md) at zero does not exist. Thus the displayed [divergence](../../../../../../divergence.md) has no classical value at the origin.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
