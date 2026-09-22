<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The balanced [comparison tournament](../../../../../comparison-tournament.md) uses

$$
C(n)=2C(n/2)+1,\qquad C(1)=0,
$$

so $C(n)=n-1$. The second-largest search compares $m=\log_2n$ direct losers, using $m-1$ comparisons. The record of $s$ contains at most $m-1$ direct losers, because $s$ loses before becoming the overall winner. Hence the third candidate set has size at most $2m-2$, requiring at most $2m-3$ comparisons.

For $n=2^m\geq4$, the complete comparison count is therefore

$$
\boxed{(n-1)+(m-1)+(2m-3)=n+3\log_2n-5.}
$$

This is $n+O(\log n)$ and therefore meets the requested $O(n+\log^2n)$ bound. The defeat-record lists can be linked in constant local work per merge; flattening the final partition takes $O(n)$ work. Thus the method also has linear overall [running time](../../../../../running-time.md) under constant-cost key comparisons.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
