<h1 id="11d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the necessity in the [differentiability of the square of a continuous function](../../../../../../differentiability-of-the-square-of-a-continuous-function.md), suppose $g=f^2$ is [differentiable](../../../../../../differentiable-function.md) at $x$. If $f(x)\ne0$, [continuity](../../../../../../continuous-function.md) makes $f(x+h)+f(x)$ nonzero for small $h$, and

$$
\frac{f(x+h)-f(x)}h
=\frac{g(x+h)-g(x)}{h[f(x+h)+f(x)]}
\longrightarrow\frac{g'(x)}{2f(x)}.
$$

Hence $f$ is [differentiable](../../../../../../differentiable-function.md) at $x$, giving alternative (i).

If $f(x)=0$, $g(x)=0$ is a minimum because $g\geq0$. The right difference quotients of $g$ are nonnegative and the left ones are nonpositive; since their common limit exists, it must be zero. Thus $g'(x)=0$, and

$$
\frac{f(x+h)^2}{|h|}
=\operatorname{sgn}(h)\frac{g(x+h)-g(x)}h\longrightarrow0.
$$

Taking square roots of this nonnegative expression shows $f(x+h)/\sqrt{|h|}\to0$, giving alternative (ii). The two labelled parts below establish sufficiency of the respective alternatives. Together they prove the full stated equivalence, including the zero of $f$ where squaring can remove a failure of [differentiability](../../../../../../differentiability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
