<h1 id="s/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use four [vertices](../../../../../vertex-graph-theory.md), with lengths $a_{12}=a_{24}=0$, $a_{23}=a_{32}=-1$, and every other non-loop arc of length $100$. The two arcs between $2$ and $3$ form a negative-length [cycle in a graph](../../../../../cycle-in-a-graph.md). For $i=1$, $j=4$, $k=3$,

$$
u_{14}^{(2)}=0,\qquad u_{13}^{(2)}=-1,\qquad u_{34}^{(2)}=-1.
$$

The recurrence would give $-2$, by concatenating $1\to2\to3$ and $3\to2\to4$. That [walk](../../../../../walk-in-a-graph.md) repeats $2$, so it is not a simple [graph path](../../../../../path-in-a-graph.md). Every simple [graph path](../../../../../path-in-a-graph.md) from $1$ to $4$ still has length at least zero, attained by $1\to2\to4$. Thus

$$
\boxed{u_{14}^{(3)}=0>-2,}
$$

a strict inequality in part (a).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [S](../../../s.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
