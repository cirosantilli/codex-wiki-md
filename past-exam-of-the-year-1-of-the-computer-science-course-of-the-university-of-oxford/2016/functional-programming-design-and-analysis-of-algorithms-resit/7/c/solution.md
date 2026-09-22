<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Whenever an update improves $F[x]$, store `choice[x] = i`. Starting at `x = m`, repeatedly increment `count[choice[x]]` and subtract that denomination from `x`, stopping at zero. The invariant is that the selected stamps plus an optimal representation of the residual total attain the original optimum; every step reduces $F[x]$ by one. Reconstruction uses $F[m]\leq m$ steps and $O(n)$ output counters, preserving the $O(mn)$ total time bound.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
