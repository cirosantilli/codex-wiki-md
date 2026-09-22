<h1 id="5/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Maintain a residual cumulative-weight target $t$, initially $1/2$, while discarding whole partitions. Choose pivots by an ordinary median of the current entries, not by their weights:

```
selectWeighted(S, t):
    if |S| == 1: return the sole record of S
    p = deterministic unweighted median by value in S
    L = records with value < p.value
    R = records with value > p.value
    ell = sum of weights in L
    if t <= ell:
        return selectWeighted(L, t)
    if t <= ell + p.weight:
        return p
    return selectWeighted(R, t - ell - p.weight)

answer = selectWeighted(all records, 1/2)
```

The invariant is $0<t\leq\sum_{x\in S}w_x$, with the desired answer the first cumulative weight reaching $t$ inside the current ordered subset. The first branch uses `<=`, which is essential: if the target equals the total left mass, the answer is the largest appropriate left-side value, not the pivot. The other branches preserve the residual target by subtracting exactly the mass discarded on the left.

A [median of medians](../../../../../../median-of-medians.md) routine finds the exact unweighted median in deterministic [linear time](../../../../../../linear-time.md). Partitioning and summing also take [linear time](../../../../../../linear-time.md), and each recursive call retains at most $\lfloor |S|/2\rfloor$ entries. Therefore $T(n)\leq T(\lceil n/2\rceil)+O(n)=O(n)$. **The algorithm is worst-case linear**, not merely expected linear under a random pivot. Exact comparisons to the weight threshold are assumed; floating-point rounding at exactly one half would need explicit treatment.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
