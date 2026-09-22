<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Remove the [integer](../../../../../integer-split.md) requirements from the previous formulation to obtain its [linear programming relaxation](../../../../../linear-programming-relaxation.md). Give each [edge](../../../../../edge-of-a-graph.md) constraint a nonnegative [dual variable](../../../../../dual-variable.md) $y_e$, and each bound for $v\in Z$ a nonnegative [dual variable](../../../../../dual-variable.md) $z_v$. Since all right-hand sides are one, the [dual linear program](../../../../../dual-linear-program.md) is

$$
\boxed{\begin{aligned}
\text{minimize}\quad&\sum_{e\in E}y_e+\sum_{v\in Z}z_v\\
\text{subject to}\quad&\sum_{e\ni v}y_e\geq1&&v\in V\setminus Z,\\
&z_v\geq1&&v\in Z,\\
&y_e\geq0,\quad z_v\geq0.
\end{aligned}}
$$

An [integer](../../../../../integer-split.md) [feasible point](../../../../../feasible-point.md) selects a multiset of [edges](../../../../../edge-of-a-graph.md) touching every nonisolated [vertex](../../../../../vertex-graph-theory.md), together with at least one singleton for each [isolated vertex](../../../../../isolated-vertex.md). Repeated [edges](../../../../../edge-of-a-graph.md) or singleton choices can be discarded without losing coverage, so an optimum has a genuine [edge cover](../../../../../edge-cover.md) of the nonisolated part and one singleton per isolated [vertex](../../../../../vertex-graph-theory.md). **If $G$ has no [isolated vertices](../../../../../isolated-vertex.md), this is exactly an [edge cover](../../../../../edge-cover.md)**, with the objective counting selected [edges](../../../../../edge-of-a-graph.md) including any unnecessary multiplicities. The isolated-singleton extension is necessary because a [graph](../../../../../graph-split.md) with an [isolated vertex](../../../../../isolated-vertex.md) admits no ordinary [edge cover](../../../../../edge-cover.md).

This interpretation concerns [integer](../../../../../integer-split.md) feasible dual solutions. The [linear programming relaxation](../../../../../linear-programming-relaxation.md) can have fractional optima, so its value need not equal the integer [independent set](../../../../../independent-set-graph-theory.md) optimum. For example, the triangle has relaxed independent-set value $3/2$, whereas its maximum [independent set](../../../../../independent-set-graph-theory.md) has size $1$ and its minimum [edge cover](../../../../../edge-cover.md) has size $2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
