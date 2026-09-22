<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [two-pointer technique](../../../../../two-pointer-technique.md), starting at opposite ends of the ordered sequence:

```
l = 0
r = n - 1
while l < r:
    s = S[l] + S[r]
    if s == x: return (l, r)
    if s < x: l = l + 1
    else:     r = r - 1
return NONE
```

If the sum is too small, every remaining pair using `l` has sum at most $S[l]+S[r]<x$, so discard `l`. If the sum is too large, every remaining pair using `r` has sum at least $S[l]+S[r]>x$, so discard `r`. The [loop invariant](../../../../../loop-invariant.md) says that every solution not already excluded has both indices in $[l,r]$. These two elimination arguments preserve it; at termination fewer than two positions remain.

Each unsuccessful iteration decreases $r-l$ by one. Therefore the [two-sum problem](../../../../../two-sum-problem.md) is solved with

$$
\boxed{O(n)\ \text{time and }O(1)\ \text{auxiliary space}.}
$$

The condition `l < r` ensures distinct positions and handles $n<2$. Under the usual interpretation of “two distinct elements” as two different occurrences, equal values in different positions are allowed. If distinct numerical values are intended instead, reject an equality with $S[l]=S[r]$: sortedness then makes the entire remaining interval equal, so it contains no distinct-value solution. Both interpretations retain linear [time complexity](../../../../../time-complexity.md). The comparison assumes exact real-number operations, as in the stated [comparison model](../../../../../comparison-model.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
