<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

The [minimum-cost flow](../../../../../minimum-cost-flow-problem.md) problem chooses, for each directed edge $(i,j)\in E$, a flow $x_{ij}$ and solves

$$
\min_x\sum_{(i,j)\in E}C_{ij}x_{ij}
$$

subject to

$$
\sum_{j:(j,i)\in E}x_{ji}-\sum_{j:(i,j)\in E}x_{ij}=b_i,
\qquad
M_{ij}\leq x_{ij}\leq\overline M_{ij}.
$$

Feasibility requires $\sum_i b_i=0$.

Set $y_{ij}=x_{ij}-M_{ij}$. Then

$$
0\leq y_{ij}\leq\overline M_{ij}-M_{ij},
$$

and its balance [vector](../../../../../vector.md) is

$$
b_i'=b_i+\sum_jM_{ij}-\sum_jM_{ji}.
$$

The objective becomes $\sum C_{ij}y_{ij}$ plus the constant $\sum C_{ij}M_{ij}$. Translation by $M$ is a bijection between feasible flows and preserves their ordering by cost, so the transformed zero-lower-bound problem is equivalent.

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
