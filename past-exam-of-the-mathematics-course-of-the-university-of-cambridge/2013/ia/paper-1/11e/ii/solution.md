<h1 id="11e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [mean value theorem](../../../../../../mean-value-theorem.md) states that a function [continuous](../../../../../../continuous-function.md) on $[a,b]$ and [differentiable](../../../../../../differentiable-function.md) on $(a,b)$, where $a<b$, has a point $\xi\in(a,b)$ such that

$$
\boxed{f'(\xi)=\frac{f(b)-f(a)}{b-a}.}
$$

To prove it using [Rolle's theorem](../../../../../../rolle-theorem.md), subtract the secant line:

$$
h(t)=f(t)-f(a)-\frac{f(b)-f(a)}{b-a}(t-a).
$$

This function has the required [continuity](../../../../../../continuous-function.md) and [differentiability](../../../../../../differentiability.md), with $h(a)=h(b)=0$. [Rolle's theorem](../../../../../../rolle-theorem.md) gives $h'(\xi)=0$, which is exactly the claimed equation. Thus a tangent slope somewhere in the interval equals the overall secant slope.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
