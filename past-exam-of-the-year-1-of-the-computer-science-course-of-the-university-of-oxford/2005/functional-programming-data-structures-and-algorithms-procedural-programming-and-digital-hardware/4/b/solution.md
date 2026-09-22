<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Divide-and-conquer algorithms](../../../../../divide-and-conquer-algorithm.md) suit problems with largely independent, balanced subproblems and an inexpensive combination step. In [merge sort](../../../../../merge-sort.md), the two halves are independently sorted and merged in linear time. Its [recurrence relation](../../../../../recurrence-relation.md) is $T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n)$, giving $\Theta(n\log n)$ [time complexity](../../../../../time-complexity.md).

[Dynamic programming](../../../../../dynamic-programming.md) suits overlapping subproblems with a compact state description. For the [coin change problem](../../../../../coin-change-problem.md), let $C(v)$ be the minimum number of coins needed to make amount $v$. With positive denominations $D$ containing $1$,

$$
C(0)=0,\qquad C(v)=1+\min_{d\in D,\ d\leq v}C(v-d).
$$

Every optimal nonempty answer has a last coin $d$ and an optimal answer for $v-d$; otherwise replacing the remainder improves it. Filling $C(0),\ldots,C(V)$ takes $O(V|D|)$ [time complexity](../../../../../time-complexity.md) and $O(V)$ [space complexity](../../../../../space-complexity.md). Repeated amounts are computed just once. This bound is in the numeric amount $V$, not its binary input length.

A [greedy algorithm](../../../../../greedy-algorithm.md) suits problems where one can prove a [greedy-choice property](../../../../../greedy-choice-property.md). For unweighted [interval scheduling](../../../../../interval-scheduling.md), choose an interval with earliest finishing time, discard overlapping intervals, and repeat. Among optimal schedules, replace the first interval by the earliest-finishing one. The replacement finishes no later, so every later interval remains feasible. Applying the same argument to the remaining intervals proves optimality. After sorting by finish time, a single scan suffices.

These examples separate the relevant structural reasons: independent halves, repeated amount states, and an exchange argument certifying each irreversible choice.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
