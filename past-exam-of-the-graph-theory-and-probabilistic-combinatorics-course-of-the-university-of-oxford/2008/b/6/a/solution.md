<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Explore the individuals one at a time, maintaining the number of discovered but unprocessed individuals. It starts at $S_0=1$. Processing one individual removes it and adds its offspring, so

$$
S_j=1+\sum_{i=1}^j\xi_i,\qquad
\mathbb P(\xi_i=1)=p,\quad\mathbb P(\xi_i=-1)=1-p.
$$

The offspring choices make these increments independent. Exploration stops when the queue first becomes empty; every processed individual has then been counted exactly once. Hence

$$
\boxed{K=\inf\{j\ge1:S_j=0\}},
$$

with $K=\infty$ if the walk never hits zero. The increment sequence can be extended independently beyond the stopping time for probability estimates.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
