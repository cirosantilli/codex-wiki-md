<h1 id="3/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [indicator functional of a constraint set](../../../../../../../indicator-functional-of-a-constraint-set.md) restricts the conjugate supremum to $[-1,1]$. Complete the square:

$$
px-\frac{x^2}{2}=\frac{p^2}{2}-\frac{(x-p)^2}{2}.
$$

Its maximizer is $x=p$ when $|p|\leq1$, and the nearer endpoint $x=\operatorname{sign}(p)$ otherwise. The [convex conjugate of a constrained quadratic](../../../../../../../convex-conjugate-of-a-constrained-quadratic.md) is therefore

$$
\boxed{E^*(p)=\begin{cases}\frac12p^2,&|p|\leq1,\\|p|-\frac12,&|p|>1.\end{cases}}
$$

This is the unit-threshold [Huber loss](../../../../../../../huber-loss.md); both branches and their first derivatives agree at the transition points. The original PDF constrains $|x|\leq1$, including both signs; the damaged TeX loses that absolute value.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
