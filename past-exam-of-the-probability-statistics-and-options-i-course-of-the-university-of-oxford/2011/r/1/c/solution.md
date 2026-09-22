<h1 id="r/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Within each connected component with $n_i$ vertices, grow a tree by starting at one vertex and repeatedly adding an edge to an unreached vertex. Connectedness guarantees such an edge until every vertex has been reached. Exactly $n_i-1$ edges are added, so the component contains at least that many edges. Summing over the $k$ components gives

$$
\boxed{m\geq\sum_{i=1}^k(n_i-1)=n-k.}
$$

The selected trees form a [spanning forest](../../../../../spanning-forest.md), and equality holds precisely when the original graph itself is a forest.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [R](../../../r.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
