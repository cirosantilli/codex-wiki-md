<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Substitute the [dual linear program](../../../../../../dual-linear-program.md) from the previous part and optimize jointly over $x,t,s$. The result is

$$
\boxed{
\begin{aligned}
\operatorname{minimize}\quad&kt+\sum_{i=1}^n s_i\\
\text{over}\quad&x\in\mathbb R^n,\ t\in\mathbb R,\ s\in\mathbb R^n\\
\text{subject to}\quad&Ax=b,\\
&s_i\geq0,\quad s_i+t\geq x_i\quad(1\leq i\leq n).
\end{aligned}}
$$

The objective is linear, and the constraints are equalities or inequalities between [affine functions](../../../../../../affine-function.md), so this is a [linear program](../../../../../../linear-programming.md). For each fixed feasible $x$, minimizing over $t,s$ gives exactly $f_k(x)$ by the [threshold formula for the sum of the largest components](../../../../../../threshold-formula-for-the-sum-of-the-largest-components.md); hence the reformulation preserves the optimal value and optimal $x$ whenever an optimum exists.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
