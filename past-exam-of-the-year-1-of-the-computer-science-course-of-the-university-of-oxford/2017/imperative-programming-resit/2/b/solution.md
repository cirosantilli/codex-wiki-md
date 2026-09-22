<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Scan candidate output integers in increasing order while maintaining the smallest possible witness:

```
spectrum(r,n):
    k = 1
    for i = 1,...,n-1:
        while r*k*k < i*i:
            k = k+1
        if r*k*k < (i+1)*(i+1):
            Out.Int(i)
```

The inner loop supplies the left inequality from part (a), and the final test checks the strict right inequality. This prints each qualifying integer once. The witness index never decreases and is at most $i$ after the inner loop, so its total number of increments is at most $n-1$. Consequently the whole nonrecursive program uses **$O(n)$ integer arithmetic operations**, not $O(n)$ iterations of a fresh search. Exact products or overflow-safe comparisons are required; arbitrary-precision bit costs depend on operand sizes.

## ↑ Ancestors (12)

1. [B](../b.md)
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
