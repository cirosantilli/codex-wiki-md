<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [vertex cover](../../../../../vertex-cover.md) of an [undirected graph](../../../../../undirected-graph.md) $G=(V,E)$ is a [subset](../../../../../subset.md) $C\subseteq V$ containing at least one endpoint of every [edge](../../../../../edge-of-a-graph.md). The optimization version of the [vertex cover](../../../../../vertex-cover.md) problem minimizes $|C|$; the [vertex cover decision problem](../../../../../vertex-cover-decision-problem.md) asks whether a cover of size at most a given bound exists.

Let $x_v=1$ mean that [vertex](../../../../../vertex-graph-theory.md) $v$ is selected. An [integer program](../../../../../integer-programming.md) for minimum-size [vertex cover](../../../../../vertex-cover.md) is

$$
\boxed{
\begin{aligned}
\min\quad&\sum_{v\in V}x_v\\
\text{subject to}\quad&x_u+x_v\geq1&& (uv\in E),\\
&x_v\in\{0,1\}&& (v\in V).
\end{aligned}}
$$

The [linear programming relaxation](../../../../../linear-programming-relaxation.md) replaces $x_v\in\{0,1\}$ by $0\leq x_v\leq1$. The [edge](../../../../../edge-of-a-graph.md) inequalities enforce coverage, and the [objective function](../../../../../objective-function.md) counts selected [vertices](../../../../../vertex-graph-theory.md) in the [integer program](../../../../../integer-programming.md).

For a [graph triangle](../../../../../triangle-in-a-graph.md) with [vertices](../../../../../vertex-graph-theory.md) $1,2,3$, the three covering constraints are

$$
x_1+x_2\geq1,\qquad x_2+x_3\geq1,\qquad x_3+x_1\geq1.
$$

Adding them gives $2(x_1+x_2+x_3)\geq3$. Therefore the relaxed [objective function](../../../../../objective-function.md) is at least $3/2$. The [feasible solution](../../../../../feasible-point.md) $x_1=x_2=x_3=1/2$ attains that lower bound, so

$$
\boxed{\operatorname{OPT}_{\mathrm{LP}}=\frac32.}
$$

In contrast, one [vertex](../../../../../vertex-graph-theory.md) leaves the opposite [edge](../../../../../edge-of-a-graph.md) uncovered and any two [vertices](../../../../../vertex-graph-theory.md) cover all three [edges](../../../../../edge-of-a-graph.md), giving integer optimum $2$. The example exhibits a genuinely non-integer optimal value, rather than merely a fractional [feasible solution](../../../../../feasible-point.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
