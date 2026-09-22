<h1 id="21h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Lagrange sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) says that if a feasible point $x^*$ and nonnegative multipliers satisfy complementary slackness and $x^*$ globally maximizes the [Lagrangian function in constrained optimization](../../../../../../lagrangian-function-in-constrained-optimization.md), then $x^*$ globally solves the constrained maximization problem. Indeed, for every feasible $x$, the signs of the constraints give $f(x)\leq L(x)\leq L(x^*)=f(x^*)$. Concavity and the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) are a common way to verify the global Lagrangian maximum.

For fixed $y$, A maximizes

$$
F(x,y)=\sum_i u_i\frac{x_i-y_i}{x_i+y_i}
=\sum_i u_i-2\sum_i\frac{u_iy_i}{x_i+y_i}
$$

subject to $x_i\geq0$ and $\sum_i x_i=X$. This is a [concave function](../../../../../../concave-function.md) of $x$. On every active coordinate, the multiplier equation is

$$
\frac{2u_iy_i}{(x_i+y_i)^2}=\lambda.
$$

Thus A's optimal allocation is given by the [water-filling algorithm](../../../../../../water-filling-algorithm.md):

$$
\boxed{x_i=\left(\sqrt{\frac{2u_iy_i}{\lambda}}-y_i\right)_+,}
$$

where $\lambda>0$ is chosen so that $\sum_i x_i=X$. Coordinates with zero expression receive no resource. This is a [water-filling algorithm](../../../../../../water-filling-algorithm.md). The formula gives the optimum when every $y_i>0$. If $y_i=0$, any $x_i>0$ already gives A the whole market $u_i$ in that region, so A assigns such coordinates arbitrarily small positive amounts and applies water filling to the remaining budget; without a convention for $0/0$, the resulting value can be a supremum rather than an attained maximum.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
