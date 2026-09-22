<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $a,w,g,r$ for the agent, monster, gold and arrow, and abbreviate $sq_{ij}$ to $s_{ij}$. A physically safe [STRIPS](../../../../../strips.md) plan is

$$
\begin{aligned}
&\operatorname{Move}(a,s_{11},s_{21}),\quad \operatorname{Move}(a,s_{21},s_{22}),\\
&\operatorname{Shoot}(a,s_{22},r,w,s_{23}),\\
&\operatorname{Move}(a,s_{22},s_{23}),\quad \operatorname{Move}(a,s_{23},s_{13}),\\
&\operatorname{Take}(a,g,s_{13}),\\
&\operatorname{Move}(a,s_{13},s_{23}),\quad \operatorname{Move}(a,s_{23},s_{22}),\\
&\operatorname{Move}(a,s_{22},s_{21}),\quad \operatorname{Move}(a,s_{21},s_{11}).
\end{aligned}
$$

Every movement follows a listed adjacency [predicate](../../../../../predicate.md). The shot is taken from $s_{22}$ while the arrow is held, and kills the monster before entry into $s_{23}$. The pit at $s_{12}$ is never entered. The pickup establishes possession of the gold, and the last four movements restore the exit location while preserving that possession. Thus **ten actions achieve the formal goal and the intended safe return**; arriving at the exit is the source model’s representation of leaving.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
