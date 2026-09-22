<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use positive integral item weights and a nonnegative integral capacity. For the [unbounded knapsack problem](../../../../../unbounded-knapsack-problem.md), define $K(c)$ to be the best value with total weight _at most_ $c$. Then

$$
\boxed{K(c)=\max\bigl(\{0\}\cup\{v_i+K(c-w_i):1\le i\le n,\ w_i\le c\}\bigr),\quad K(0)=0.}
$$

The zero candidate is the empty selection, so unused capacity is allowed and an empty set of fitting items causes no problem. Every nonempty feasible selection has some last item $i$; removing one copy leaves a feasible solution at capacity $c-w_i$. Its value is bounded by the corresponding candidate. Conversely, taking an optimal smaller selection and adding that item attains the candidate, proving the [recurrence relation](../../../../../recurrence-relation.md) by [optimal substructure](../../../../../optimal-substructure.md). Positive weights make every dependency strictly smaller.

Fill capacities in increasing order. There are $W+1$ entries, each scanning $n$ items, so the [dynamic programming](../../../../../dynamic-programming.md) takes $O(nW)$ time and $O(W)$ storage. A winning item pointer at each capacity reconstructs the chosen multiplicities. These are capacity-dependent, [pseudopolynomial](../../../../../pseudopolynomial-time.md) bounds. For zero-weight items, any positive value makes the repetition problem unbounded; nonpositive-value zero-weight items may simply be discarded before using the recurrence.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
