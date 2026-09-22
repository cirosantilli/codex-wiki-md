<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [binary search](../../../../../binary-search.md) for the least positive integer $k$ whose square reaches the lower bound:

```
test(i,r):
    lo = 1; hi = i
    while lo < hi:
        mid = lo + (hi-lo)//2
        if r*mid*mid < i*i:
            lo = mid+1
        else:
            hi = mid
    return r*lo*lo < (i+1)*(i+1)
```

The search interval is valid because $ri^2\geq i^2$. Once the least witness is located, the final strict upper test decides membership, by part (a). No recursion or approximate square root is used.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
