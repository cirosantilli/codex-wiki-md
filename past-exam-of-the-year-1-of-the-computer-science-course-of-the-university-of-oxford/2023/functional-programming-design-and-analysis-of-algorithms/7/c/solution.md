<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take

$$
\boxed{S=(2,4,1,3).}
$$

Its longest [strictly increasing subsequences](../../../../../strictly-increasing-subsequence.md) have length two. A subsequence starting with $2$ can continue with $4$ or with $3$, but cannot use both in increasing order; one starting at $1$ has only $3$ after it.

The specified [greedy algorithm](../../../../../greedy-algorithm.md) may choose the longest increasing subsequence $(2,3)$. The remaining sequence is $(4,1)$, which needs two singleton increasing subsequences. The algorithm then uses **three** subsequences in total.

However, $(2,4)$ and $(1,3)$ partition the original sequence into **two** increasing subsequences. One is impossible because the original sequence is not increasing. Hence two is optimal and the greedy choice is suboptimal. This establishes the [counterexample to removing a longest increasing subsequence](../../../../../counterexample-to-removing-a-longest-increasing-subsequence.md) without relying on a tie-breaking rule: the problem asks for a longest choice that can fail.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
