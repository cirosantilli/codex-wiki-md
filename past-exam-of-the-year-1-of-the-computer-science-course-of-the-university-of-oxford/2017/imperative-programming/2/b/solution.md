<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep the target as an absolute, zero-based array index:

```
function Find(i; var a; l, r): T
    require l <= i < r
    Partition(a,l,r,m,n)
    if i < m then
        return Find(i,a,l,m)
    else if i >= n then
        return Find(i,a,n,r)
    else
        return a[i]
```

The [order statistic](../../../../../order-statistic.md) belongs to the lower segment, equality interval or upper segment according to the index comparison. In the middle interval its value is the pivot; otherwise [Quickselect](../../../../../quickselect.md) recurses only into the relevant outer interval. The nonempty equality interval guarantees a strictly shorter retained segment. The procedure sorts neither discarded segment. Since indices remain absolute, the right recursion does not subtract `n` from `i`.

## ↑ Ancestors (12)

1. [B](../b.md)
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
