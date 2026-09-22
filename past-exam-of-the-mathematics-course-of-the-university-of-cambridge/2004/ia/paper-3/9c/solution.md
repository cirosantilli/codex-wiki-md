<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Set $r=\sqrt{x^2+y^2}$. The bound $|xy|\leq r^2/2$ and $|x^2-y^2|\leq r^2$ give $|f(x,y)|\leq r^2/2$. Hence $f\to0$ at the origin, proving [continuity](../../../../../continuous-function.md), and $|f(x,y)|/r\to0$, proving [Fréchet differentiability](../../../../../frechet-differentiability.md) there with **derivative equal to the zero linear map**.

Along the coordinate axes, direct difference quotients give

$$
\boxed{f_x(0,y)=-y,\qquad f_y(x,0)=x.}
$$

These formulas include the origin. Therefore the two [mixed partial derivatives](../../../../../mixed-partial-derivative.md) differ:

$$
\boxed{\partial_y(\partial_x f)(0,0)=-1,\qquad\partial_x(\partial_y f)(0,0)=1.}
$$

The explicit operator order removes any ambiguity about the notation for mixed derivatives. Also $f_{xx}(0,0)=f_{yy}(0,0)=0$, since the first derivatives restricted to their own axes vanish identically.

All four second-order [partial derivatives](../../../../../partial-derivative.md) are discontinuous at the origin. Away from it,

$$
f_{xx}(x,y)=\frac{4xy^3(-x^2+3y^2)}{(x^2+y^2)^3},\qquad f_{yy}(x,y)=-\frac{4yx^3(-y^2+3x^2)}{(x^2+y^2)^3}.
$$

Along $x=y\ne0$ these are one and minus one, rather than their zero values at the origin. Meanwhile $\partial_y\partial_xf(x,0)=1$ for $x\ne0$, whereas its value at the origin is minus one; and $\partial_x\partial_yf(0,y)=-1$ for $y\ne0$, whereas its origin value is one. This gives a concrete [unequal mixed partial derivatives](../../../../../unequal-mixed-partial-derivatives.md) example despite differentiability of the original function.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
