<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [unbounded knapsack problem](../../../../../unbounded-knapsack-problem.md), let $F(c)$ be the greatest total value obtainable with weight at most capacity $c$. Assume positive integer item weights and nonnegative integer capacity $W$. Set $F(0)=0$, and fill increasing capacities using

$$
F(c)=\max\bigl(\{0\}\cup\{v_i+F(c-w_i):w_i\leq c\}\bigr).
$$

The zero alternative permits unused capacity. If a nonempty optimum includes item $i$, removing one copy leaves a feasible smaller-capacity instance; its remaining value cannot exceed $F(c-w_i)$. Conversely every candidate in the displayed maximum is feasible, proving equality. The smaller-capacity state allows the same type again, implementing repetition.

The answer is **$F(W)$, computed in $O(nW)$ time and $O(W)$ space**. Record an attaining item at each state to reconstruct the multiset. This is [pseudopolynomial time](../../../../../pseudopolynomial-time.md), because $W$ is a number whose binary representation may have only $O(\log W)$ bits. A positive-value zero-weight type would make the optimum unbounded and must be excluded or detected separately.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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
