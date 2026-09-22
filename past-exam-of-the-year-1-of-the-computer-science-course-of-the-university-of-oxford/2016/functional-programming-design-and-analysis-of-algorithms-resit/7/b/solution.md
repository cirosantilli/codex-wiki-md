<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $F[x]$ be the minimum number of stamps for total $x$. Since denomination 1 is available, every nonnegative total is reachable. The [dynamic programming recurrence](../../../../../dynamic-programming-recurrence.md) is

$$
F[0]=0,\qquad F[x]=1+\min_{d_i\leq x}F[x-d_i]\quad(x\geq1).
$$

Fill the table in increasing order of $x$:
```
F[0] = 0
for x = 1,...,m:
    F[x] = infinity
    for i = 1,...,n:
        if d[i] <= x:
            F[x] = min(F[x], 1 + F[x-d[i]])
return F[m]
```
Every representation of $x$ has a last stamp $d_i$, so its remaining count is at least $F[x-d_i]$. Conversely, appending $d_i$ to an optimal residual representation attains each candidate. Thus the recurrence is exact by the [principle of optimality](../../../../../principle-of-optimality.md). Worst-case time is **$O(mn)$**, with $O(m)$ storage. This is [pseudo-polynomial time](../../../../../pseudo-polynomial-time.md) in the numerical target, rather than polynomial time in its binary encoding length.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
