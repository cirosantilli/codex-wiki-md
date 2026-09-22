<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) with the sign convention

$$
L(x,\lambda)=3x_1-x_2+2x_3^2+\lambda(x_1^2+x_2^2+x_3-2).
$$

For every $\lambda>0$, this is a [strictly convex](../../../../../../strictly-convex-function.md) quadratic in $x$, with unique global minimizer

$$
x_1(\lambda)=-\frac3{2\lambda},\qquad x_2(\lambda)=\frac1{2\lambda},\qquad x_3(\lambda)=-\frac\lambda4.
$$

These formulas follow by setting the three partial derivatives of the [optimization Lagrangian](../../../../../../optimization-lagrangian.md) to zero; its [Hessian](../../../../../../hessian-matrix.md) is $\operatorname{diag}(2\lambda,2\lambda,4)$, which is [positive-definite](../../../../../../positive-definite-bilinear-form.md).

Choose $\lambda>0$ to make this minimizer feasible. Its constraint value is $5/(2\lambda^2)-\lambda/4$, so the scalar equation is

$$
\frac5{2\lambda^2}-\frac\lambda4=2,\qquad\text{equivalently}\qquad\lambda^3+8\lambda^2-10=0.
$$

The left side of the first equation is strictly decreasing on $(0,\infty)$, with limits $+\infty$ and $-\infty$. Thus exactly one positive multiplier exists and can be obtained by a bracketed scalar root search. The [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) proves that its associated feasible point is the global optimum; strict Lagrangian [convexity](../../../../../../convex-function.md) makes that optimum unique.

Consequently **the unique solution is**

$$
\boxed{x^*=\left(-\frac3{2\lambda},\frac1{2\lambda},-\frac\lambda4\right),\quad\lambda>0,\quad\lambda^3+8\lambda^2-10=0.}
$$

Its objective value is $-5/\lambda+\lambda^2/8$. This [scalar multiplier certificate for a quadratic equality constraint](../../../../../../scalar-multiplier-certificate-for-a-quadratic-equality-constraint.md) does not require finding the multiplier in radicals, and does not mistake the nonconvex equality surface for a [convex set](../../../../../../convex-set.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
