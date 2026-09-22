<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On a worst-case branch, the described sequential quarter-point tests make three equality tests per reduction, giving $Q(n)=Q(n/4)+3$ until constant size. Thus $Q(4^k)=3k+O(1)$. Ordinary [binary search](../../../../../binary-search.md) makes one equality test per halving: $B(n)=B(n/2)+1$, so $B(4^k)=2k+O(1)$.

**Both searches take $\Theta(\log n)$ time, but the specified quaternary search uses asymptotically $3/2$ as many equality tests.** A quarter-sized branch does not compensate for the three sequential pivots. The numerical ratio concerns precisely the unit equality-test model in the paper; counting ordering comparisons, array accesses or a differently arranged pivot decision tree requires its own constants.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
