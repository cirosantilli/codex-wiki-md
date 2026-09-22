<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $P$ for the [prime numbers](../../../../../../prime-number-split.md) in $A$ and $C=A\setminus P$ for its nonprime elements. Since $n\geq4$, both [antichains](../../../../../../antichain.md) have at least two elements: $2,3\in P$ and $1,4\in C$. Every element of $P$ is below every element of $C$. We can classify a [subset](../../../../../../subset.md) $S$ by its intersection with these two levels of the [two-level partial order](../../../../../../two-level-partial-order.md).

- If $S=\varnothing$, every element of $A$ is an [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md). There is no [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md), because $S$ has no elements, and no [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md), because the distinct elements $2,3$ are incomparable minimal elements of $A$.
- If $S=\{p\}$ with $p\in P$, its [upper bounds](../../../../../../upper-bound-in-a-partially-ordered-set.md) are $\{p\}\cup C$; its [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) and [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) are both $p$.
- If $S\subseteq P$ has at least two elements, its [upper bounds](../../../../../../upper-bound-in-a-partially-ordered-set.md) are exactly $C$. There is no [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) in $S$ and no [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md), because $C$ has at least two incomparable elements.
- If $S\cap C=\{c\}$, its only [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md) is $c$: no different element is above this nonprime element. Since every remaining element of $S$ is a [prime number](../../../../../../prime-number-split.md), $c$ belongs to $S$ and dominates all of it. Thus $c$ is both its [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) and its [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md).
- If $S$ contains at least two elements of $C$, these distinct nonprime elements have no common [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md), and $S$ has neither a [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) nor a [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md).

Consequently **an [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md) exists exactly when $|S\cap C|\leq1$; a [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) or [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) exists exactly when $|S\cap C|=1$ or $S$ is a singleton [subset](../../../../../../subset.md) of $P$**. The exhaustive cases also justify why the last two existence criteria coincide here.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
