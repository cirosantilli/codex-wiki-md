<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume job sizes $t_i\geq0$ and machine speeds $s_j>0$, with at least one machine. Let $y_{ij}\geq0$ be the amount of job $T_i$ assigned to machine $M_j$, and let $T\geq0$ be the proposed [makespan](../../../../../makespan.md). Use the [linear program](../../../../../linear-programming-split.md)

$$
\boxed{
\begin{aligned}
\min\quad&T\\
\text{subject to}\quad&\sum_{j=1}^m y_{ij}=t_i&& (1\leq i\leq n),\\
&\sum_{i=1}^n y_{ij}\leq s_jT&& (1\leq j\leq m),\\
&y_{ij}\geq0&& (1\leq i\leq n,\ 1\leq j\leq m),\\
&T\geq0.
\end{aligned}}
$$

The first family of constraints assigns every job completely. The second bounds each machine's completion time by $T$, since $L_j/s_j\leq T$ is equivalent to $L_j\leq s_jT$. It is a [linear inequality](../../../../../linear-inequality.md) because $s_j$ is an input constant. There is no integrality restriction: jobs are divisible as specified in this [scheduling](../../../../../scheduling.md) model.

To verify the formulation, any actual allocation defines the variables above, with $T$ equal to its largest completion time, and satisfies every constraint. Conversely, from a [feasible solution](../../../../../feasible-point.md), assign amount $y_{ij}$ to machine $M_j$ and process its assigned pieces consecutively. Its total time is at most $T$, so the [linear program](../../../../../linear-programming-split.md) realizes the claimed [makespan](../../../../../makespan.md).

There is also a useful exact check. Put $W=\sum_i t_i$ and $S=\sum_j s_j$. Summing machine constraints gives $W\leq ST$, so $T\geq W/S$. Assigning

$$
y_{ij}=t_i\frac{s_j}{S}
$$

makes every machine's completion time $W/S$, proving

$$
\boxed{T^*=\frac{\sum_i t_i}{\sum_j s_j}.}
$$

This relies on the paper's divisible-work model, in which machine completion times depend only on total assigned size. If $W=0$, the optimum is $0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
