<h1 id="s/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Before a potential update, let $S$ be the reached rows and $T$ the reached columns in an alternating forest grown from unmatched rows. Every reached column is matched, or an augmentation would already have occurred, and its matched row is reached. Each [tree](../../../../../tree-graph-theory-split.md) has one more reached row than reached column, so $|S|-|T|>0$.

The update amount is the smallest slack across $S\times T^c$. It is strictly positive because all zero-slack [edges](../../../../../edge-of-a-graph.md) have already been explored, and the complete [assignment problem](../../../../../assignment-problem.md) guarantees that the set is nonempty before a [perfect matching](../../../../../perfect-matching.md) is found. Increasing $u_i$ for $i\in S$ and decreasing $v_j$ for $j\in T$ therefore increases the dual sum by

$$
\boxed{\Delta(|S|-|T|)>0.}
$$

All feasibility inequalities remain valid by the definition of the minimum slack.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
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
