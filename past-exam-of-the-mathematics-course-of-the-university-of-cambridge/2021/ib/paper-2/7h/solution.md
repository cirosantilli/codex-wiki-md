<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Introduce slack variables $s_1,s_2,s_3$. In the initial [simplex algorithm](../../../../../simplex-algorithm.md) dictionary, $x_2$ has the largest positive objective coefficient. The ratio test gives

$$
\min\left\{\frac73,\frac52,\frac21\right\}=2,
$$

so $x_2$ enters and $s_3$ leaves. Solving the third constraint for $x_2$ gives

$$
x_2=2-x_1-2x_3-s_3.
$$

The objective becomes

$$
z=3x_1+6x_2+4x_3
=12-3x_1-8x_3-6s_3.
$$

Every reduced cost is now nonpositive, so the simplex optimality criterion gives

$$
\boxed{(x_1,x_2,x_3)=(0,2,0),\qquad z_{\max}=12}.
$$

The other two slacks both equal one.

The [dual linear program](../../../../../dual-linear-program.md) is

$$
\begin{aligned}
\text{minimize}\quad&7y_1+5y_2+2y_3,\\
\text{subject to}\quad
&2y_1+4y_2+y_3\geq3,\\
&3y_1+2y_2+y_3\geq6,\\
&y_1+2y_2+2y_3\geq4,\\
&y_1,y_2,y_3\geq0.
\end{aligned}
$$

The vector

$$
\boxed{(y_1,y_2,y_3)=(0,0,6)}
$$

is dual feasible and has objective value $12$. By [weak duality](../../../../../weak-duality.md), it and the displayed primal point are optimal; they also satisfy [complementary slackness](../../../../../complementary-slackness.md).

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
