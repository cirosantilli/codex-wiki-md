<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Each recursive call is a [tail call](../../../../../tail-call.md): nothing remains to be computed after it returns. Replace it by an update of the retained bounds:

```
function Select(i; var a; N): T
    require 1 <= i <= N
    target := i-1
    l := 0
    r := N
    while true do
        Partition(a,l,r,m,n)
        if target < m then
            r := m
        else if target >= n then
            l := n
        else
            return a[target]
```

The [loop invariant](../../../../../loop-invariant.md) retains the target [order statistic](../../../../../order-statistic.md) in $[l,r)$ with $l\leq target<r$. Each nonreturning iteration strictly decreases $r-l$, because $[m,n)$ is nonempty. This proves termination and replaces recursive stack space by **$O(1)$ auxiliary space**, apart from the pivot routine's own storage.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
