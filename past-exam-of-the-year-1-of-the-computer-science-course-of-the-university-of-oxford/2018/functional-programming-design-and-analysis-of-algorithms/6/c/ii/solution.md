<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [minimum coin change recurrence](../../../../../../minimum-coin-change-recurrence.md), initialize $C(0)=0$ and use

$$
C(a)=1+\min_{i:v_i\leq a} C(a-v_i),
$$

where the minimum over no feasible predecessor is $\infty$ and $1+\infty=\infty$. Removing the last coin of an optimal representation proves the lower bound; appending the corresponding coin to an optimal predecessor proves attainability. **$C(v)$ is the minimum number of coins**, obtained in $O(nv)$ time and $O(v)$ space. Store one minimizing coin per amount if the actual coins are wanted.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
