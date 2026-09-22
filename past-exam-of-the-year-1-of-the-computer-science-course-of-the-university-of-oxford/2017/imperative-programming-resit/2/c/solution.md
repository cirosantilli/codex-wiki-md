<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Before testing candidate $i$, every earlier integer has been printed exactly when it belongs to the spectrum, and every positive $h<k$ satisfies $rh^2<i^2$. During the inner loop that exclusion remains true: an excluded candidate is passed over only after checking its square.

At termination of the inner loop, $rk^2\geq i^2$, so $k$ is the least positive possible witness. If its square is already at least $(i+1)^2$, every larger witness is too large as well; otherwise it satisfies both required inequalities and $i$ is printed. Advancing $i$ preserves the earlier-witness exclusion because the new lower bound only increases. These [loop invariants](../../../../../loop-invariant.md) establish both completeness and absence of extra outputs.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
