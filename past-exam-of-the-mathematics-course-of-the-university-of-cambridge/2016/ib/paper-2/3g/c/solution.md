<h1 id="3g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The function $g(t)=|t|^{3/2}$ is [differentiable](../../../../../../differentiable-function.md) everywhere: for $t\ne0$, its [derivative](../../../../../../derivative.md) is $(3/2)\operatorname{sgn}(t)\sqrt{|t|}$, while at zero the difference quotient is $\operatorname{sgn}(t)\sqrt{|t|}\to0$.

The function $k(t)=|t|^{1/2}$ is [differentiable](../../../../../../differentiable-function.md) for $t\ne0$, with [derivative](../../../../../../derivative.md) $\operatorname{sgn}(t)/(2\sqrt{|t|})$. At zero its difference quotient is $\operatorname{sgn}(t)/\sqrt{|t|}$, which has no finite limit. Applying the coordinatewise-sum argument gives

$$
\boxed{f\text{ is differentiable exactly at }(x,y)\text{ with }y\ne0.}
$$

At those points,

$$
Df(x,y)(h,k)=\frac32\operatorname{sgn}(x)\sqrt{|x|}\,h+\frac{\operatorname{sgn}(y)}{2\sqrt{|y|}}\,k,
$$

where the first coefficient is zero at $x=0$. At any point with $y=0$, the restriction to the vertical coordinate line already fails to be [differentiable](../../../../../../differentiable-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3G](../../3g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
