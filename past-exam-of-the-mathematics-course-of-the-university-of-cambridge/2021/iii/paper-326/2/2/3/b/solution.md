<h1 id="2/2/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $\lambda f\in\partial J(f)$ and $1-\lambda\alpha>0$ when $\alpha<1/\lambda$, part a gives

$$
\lambda f\in\partial J((1-\lambda\alpha)f).
$$

Set $u=(1-\lambda\alpha)f$. Then

$$
0=u-f+\alpha\lambda f
\in u-f+\alpha\partial J(u).
$$

This is the [subgradient optimality condition](../../../../../../../../subgradient-optimality-condition.md) for

$$
\frac12\|u-f\|^2+\alpha J(u).
$$

The squared norm is [strictly convex](../../../../../../../../strictly-convex-function.md), so the objective has at most one minimizer. Hence

$$
\boxed{u=(1-\lambda\alpha)f}
$$

is its unique minimizer.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [2](../../../2.md)
4. [2](../../../../2.md)
5. [Paper 326](../../../../../paper-326-split.md)
6. [Iii](../../../../../split.md)
7. [2021](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
