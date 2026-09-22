<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an integer pivot $0\leq p\leq N+1$, exactly $k$ entries lie in $[0,p)$. That interval contains $p$ possible [integers](../../../../../../integer-split.md). If $k<p$, the [pigeonhole principle](../../../../../../pigeonhole-principle.md) implies that **some value in $[0,p)$ is missing**. Counting occurrences rather than distinct entries only strengthens this argument: $k$ occurrences cannot cover more than $k$ distinct values.

For completeness, if $p>N+1$ the lower side contains the entire permitted value range, which already has a missing value. If $p\leq0$, the condition $k<p$ is impossible. Thus the general conclusion is a missing permitted value below $p$; an internal pivot gives useful localization.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Imperative programming resit](../../../../imperative-programming-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
