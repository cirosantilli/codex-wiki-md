<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

During the computation in part i, record an index $\operatorname{last}[t]$ attaining the minimum at every positive amount. Starting with $t=v$, print $x_{\operatorname{last}[t]}$ and replace $t$ by $t-x_{\operatorname{last}[t]}$, continuing until $t=0$.

Every step decreases the amount and reduces the table entry by exactly one. The printed denominations therefore sum to $v$ and their number is exactly $M[v]$, proving optimality. **The total [running time](../../../../../../running-time.md) is $O(nv+M[v])$**, including the output; $M[v]\le v$ because denomination $1$ is available. The predecessor [array](../../../../../../array-data-structure.md) adds $O(v)$ to the [space complexity](../../../../../../space-complexity.md). This is reconstruction from the [dynamic programming](../../../../../../dynamic-programming.md) certificate, not the largest-denomination [greedy algorithm](../../../../../../greedy-algorithm.md), which need not be optimal for arbitrary denominations.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
