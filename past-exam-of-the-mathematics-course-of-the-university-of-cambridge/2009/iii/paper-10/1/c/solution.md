<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $p(y)=D_yf(x)$. Rescaling the parameter in the [directional derivative](../../../../../../directional-derivative.md) gives $p(ay)=ap(y)$ for $a>0$, and $p(0)=0$ handles $a=0$. For sufficiently small $t>0$, [convexity](../../../../../../convex-function.md) gives

$$
f(x+t(y+z))\leq\tfrac12f(x+2ty)+\tfrac12f(x+2tz).
$$

Subtract $f(x)$, divide by $t$, and let $t\downarrow0$. The finite limits from part (b) give

$$
\boxed{p(y+z)\leq p(y)+p(z),\qquad p(ay)=ap(y)\quad(a\geq0).}
$$

These are exactly the defining conditions of a [sublinear functional](../../../../../../sublinear-function.md). In particular, a [directional derivative of a convex function is sublinear](../../../../../../directional-derivative-of-a-convex-function-is-sublinear.md); it need not be linear.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
