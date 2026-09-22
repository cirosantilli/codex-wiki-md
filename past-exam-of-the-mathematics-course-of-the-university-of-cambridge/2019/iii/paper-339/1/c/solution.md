<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep $y\geq0$ as the domain restriction, introduce nonnegative [Lagrange multipliers](../../../../../../lagrange-multiplier.md) $s_i$ for $y_i\leq1$, and introduce a free multiplier $t\in\mathbb R$ for $\sum_i y_i=k$. The maximizing [Lagrangian](../../../../../../lagrangian.md) is

$$
L(y,s,t)=x^Ty+s^T(\mathbf1-y)+t(k-\mathbf1^Ty)
=\mathbf1^Ts+kt+(x-s-t\mathbf1)^Ty.
$$

Its supremum over $y\geq0$ is finite exactly when $s+t\mathbf1\geq x$, and then equals $kt+\sum_i s_i$. By [linear programming duality](../../../../../../linear-programming-duality.md), since the primal is feasible and bounded,

$$
\boxed{f_k(x)=\min_{t\in\mathbb R,\ s\in\mathbb R^n}\left\{kt+\sum_i s_i:s_i\geq0,\ s_i+t\geq x_i\right\}.}
$$

Minimizing over $s$ for fixed $t$ gives $s_i=(x_i-t)_+$, the [positive part of a real-valued function](../../../../../../positive-part-of-a-real-valued-function.md). Thus the [threshold formula for the sum of the largest components](../../../../../../threshold-formula-for-the-sum-of-the-largest-components.md) is

$$
\boxed{f_k(x)=\min_{t\in\mathbb R}\left[kt+\sum_i(x_i-t)_+\right].}
$$

For a direct attainment check, order the coordinates $x_{[1]}\geq\cdots\geq x_{[n]}$. Any $t\in[x_{[k+1]},x_{[k]}]$ is optimal for $k<n$, while any $t\leq x_{[n]}$ is optimal for $k=n$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
