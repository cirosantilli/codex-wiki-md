<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After one jump, the largest reachable index is two. After at most two jumps, the reachable indices form the prefix $[0,5]$: index two can reach five, but no reachable departure before that second jump can go further. From indices zero through five, the largest endpoint of one further jump is $4+A[4]=9$. Thus three jumps cannot reach index ten.

The two routes

$$
\boxed{0\to2\to4\to8\to10\quad\text{and}\quad0\to2\to4\to9\to10}
$$

are valid and use four jumps. Therefore $\boxed{\text{the minimum is four jumps, and the minimizing route is not unique}}$. The frontier argument proves the lower bound independently of merely exhibiting a route. In fact these are the two minimizing index sequences: the last departure in a four-jump solution must be eight or nine, reached in three jumps through four, which is reached in two jumps only through two.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
