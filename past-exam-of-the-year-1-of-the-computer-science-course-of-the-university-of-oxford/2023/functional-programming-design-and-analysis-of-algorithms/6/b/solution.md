<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Sort the open [intervals](../../../../../interval-mathematics.md) by increasing left endpoint. Scan them in that order, maintaining the largest right endpoint $R$ among previously seen intervals. For the next interval $(a,b)$, report an intersection if **$a<R$**; otherwise set $R=\max(R,b)$ and continue. Equality is allowed: $(a,R)$ and $(R,b)$ do not meet because the intervals are open. For zero or one interval, return that they are mutually non-intersecting.

If $a<R$, a previous interval with right endpoint $R$ has left endpoint at most $a$ and has positive length. Together with $b>a$, this guarantees an interior common point. Conversely, if $a\geq R$, every earlier interval ends at or before $a$, so none intersects the new one. This [loop invariant](../../../../../loop-invariant.md) proves correctness. A [comparison sort](../../../../../comparison-sort.md) costs $O(n\log n)$ time and the scan costs $O(n)$.

For the lower bound, transform an input of integers $z_1,\ldots,z_n$ for the [element distinctness problem](../../../../../element-distinctness-problem.md) into

$$
r_i=(2z_i,2z_i+1).
$$

Equal integers produce identical, intersecting intervals. Unequal integers differ by at least one, so their intervals are disjoint. The answer therefore decides whether all the integers are distinct. Moreover, comparing any two constructed endpoints can be simulated by comparing their original integers and, only on equality, their fixed offsets $0$ or $1$. Thus the transformation preserves the [comparison model](../../../../../comparison-model.md), rather than gaining extra information from arithmetic on arbitrary endpoints. The supplied distinctness lower bound gives **$\Omega(n\log n)$ comparisons**, matching the upper bound. This is the [comparison lower bound for interval disjointness](../../../../../comparison-lower-bound-for-interval-disjointness.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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
