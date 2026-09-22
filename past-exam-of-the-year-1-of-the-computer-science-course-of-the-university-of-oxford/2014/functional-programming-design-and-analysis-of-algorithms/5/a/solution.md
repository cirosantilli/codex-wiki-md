<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [binary search](../../../../../binary-search.md). Keep the half-open interval of candidate indices $[l,r)$, initially $[0,n)$. While it is nonempty, set $p=\lfloor(l+r)/2\rfloor$ and make one [ternary comparison](../../../../../ternary-comparison.md) between the target $x$ and $S[p]$. Equality succeeds; a smaller target replaces $r$ by $p$; a larger target replaces $l$ by $p+1$. An empty interval certifies absence.

The [loop invariant](../../../../../loop-invariant.md) is that every possible occurrence of $x$ lies in the current interval. Its preservation follows from the ordering of $S$. After an unsuccessful comparison, at most $\lfloor(r-l)/2\rfloor$ candidates remain. Thus the maximum number of comparisons for $n\ge1$ satisfies $C(n)\le1+C(\lfloor n/2\rfloor)$ with $C(0)=0$, giving

$$
\boxed{C(n)\le\lfloor\log_2 n\rfloor+1=\log_2 n+O(1).}
$$

One [ternary comparison](../../../../../ternary-comparison.md) supplies all three outcomes; it is not counted as separate less-than and equality tests. The [comparison model](../../../../../comparison-model.md) abstracts away any cost of navigating a non-random-access sequence. For an [array](../../../../../array-data-structure.md), navigation also takes constant time per step.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
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
