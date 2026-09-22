<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce nonnegative slack variables $s_i$ and write $z=c^{\mathsf T}x$. A maximizing [simplex dictionary](../../../../../simplex-dictionary.md) is dual feasible when every nonbasic coefficient in the objective is nonpositive. After inserting a constraint, the [dual simplex algorithm](../../../../../dual-simplex-algorithm.md) retains this property while repairing any negative basic value. For a leaving row $x_B=\beta+\sum_j d_jx_j$ with $\beta<0$, only $d_j>0$ can enter; choose a column minimizing the ratio of its objective penalty to $d_j$.

For the first [linear program](../../../../../linear-programming.md), $x_1$ has the best profit-to-resource ratio. Pivot it into the initial slack basis to obtain

$$
x_1=5-2x_2-3x_3-4x_4-s_1,\qquad
z=5-x_2-2x_3-3x_4-s_1.
$$

All basic values are nonnegative and all reduced costs are nonpositive, so the optimal point is $(5,0,0,0)$, with value five. Adding the second constraint gives

$$
s_2=1+3x_2+4x_3+5x_4+2s_1.
$$

The same basis remains feasible and optimal: the second constraint does not change the answer.

The third constraint gives the new row

$$
s_3=-1-x_2+x_3+x_4-s_1.
$$

The current dictionary is dual feasible but primal infeasible. The eligible entering variables are $x_3,x_4$, with dual ratio-test values $2$ and $3$ respectively. Enter $x_3$ and leave $s_3$; solving that row and substituting into the old rows yields

$$
\begin{aligned}
x_3&=1+x_2-x_4+s_1+s_3,\\
x_1&=2-5x_2-x_4-4s_1-3s_3,\\
s_2&=5+7x_2+x_4+6s_1+4s_3,\\
z&=3-3x_2-x_4-3s_1-2s_3.
\end{aligned}
$$

This is a feasible optimal [simplex dictionary](../../../../../simplex-dictionary.md). Thus the new optimal point is $(2,0,1,0)$, with value three. As an independent [linear programming optimality certificate](../../../../../linear-programming-optimality-certificate.md), dual multipliers $(3,0,2)$ have weighted objective bound $3\cdot5+2(-6)=3$ and weighted coefficient row $(1,4,1,2)$, which dominates the profit row.

On inserting the fourth constraint the slack is

$$
s_4=1-x_2-2x_3-2x_4=-1-3x_2-2s_1-2s_3.
$$

It has a negative constant and no eligible entering column. Since all its nonbasic variables are nonnegative, this row cannot be satisfied: the fourth [linear program](../../../../../linear-programming.md) is infeasible, and adding the fifth constraint cannot restore feasibility. The requested optimal values are therefore

$$
\boxed{\operatorname{val}P(\{1\})=5,\quad\operatorname{val}P(\{1,2\})=5,\quad\operatorname{val}P(\{1,2,3\})=3;\quad k=4,5\text{ are infeasible}.}
$$

The arbitrary-data selection question is a [maximum feasible subsystem](../../../../../maximum-feasible-subsystem.md) problem. With rational input it is in [NP](../../../../../np-complexity.md): guess the selected row indices, and test their [linear programming](../../../../../linear-programming.md) feasibility in [polynomial time](../../../../../polynomial-time.md). Equivalently, a nonempty rational polyhedron has a feasible rational point of polynomially bounded encoding length, which serves as a certificate.

For an explicit [NP-hardness](../../../../../np-hardness.md) reduction, take an [independent set](../../../../../independent-set-graph-theory.md) instance with graph $H$ having $r$ vertices and desired independent-set size $K$. Use variables $x_v\geq0$, one inequality $-x_v\leq-1$ for each vertex, and $M=r+1$ identical copies of $x_u+x_v\leq1$ for each edge. Ask for a feasible subsystem of size $M|E(H)|+K$. An [independent set](../../../../../independent-set-graph-theory.md) of size $K$ gives such a subsystem: include all edge rows and those $K$ vertex rows, and use its indicator vector. Conversely, omitting every copy of even one edge row leaves at most $M(|E(H)|-1)+r<M|E(H)|+K$ selectable rows. Hence any qualifying subsystem retains every edge inequality and at least $K$ vertex inequalities. Their vertices must be independent, since two adjacent selected vertices would force $x_u+x_v\geq2$. The construction has polynomial size; $c$ is irrelevant to feasibility. Thus **the rational-input [decision problem](../../../../../decision-problem.md) is [NP-complete](../../../../../np-completeness.md)**, not merely difficult because there are many subsets to enumerate.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
