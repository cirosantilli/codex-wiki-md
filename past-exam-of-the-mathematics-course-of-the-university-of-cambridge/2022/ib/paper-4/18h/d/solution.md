<h1 id="18h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The dual is

$$
\boxed{\text{maximize }e^Ty
\quad\text{subject to }Ay\leq e, y\geq0},
$$

which is in standard maximization form after adding nonnegative slack variables. The simplex pivots first introduce the variable with coefficient seven and then the remaining payoff column; the optimum occurs where both constraints bind:

$$
y_1+5y_2=1,
\qquad7y_1+3y_2=1.
$$

Thus $y=(1/16,3/16)$ and the dual value is $1/4$. Complementary slackness gives $x=(1/8,1/8)$. Hence $v=4$ and the normalized optimal strategies are

$$
\boxed{p=(1/2,1/2),
\qquad q=(1/4,3/4),
\qquad v=4}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
