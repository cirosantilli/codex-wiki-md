<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Accumulate denominators while reducing the positive residual:

```
procedure fromRat(m,n; var e)
    require 0 <= m < n
    e.i := 0
    while m > 0 do
        q := n div m
        if n mod m != 0 then q := q+1
        assert e.i < N
        e.x[e.i] := q
        e.i := e.i+1
        m := m*q-n
        n := n*q
        Reduce(m,n)
```

The quotient-and-remainder calculation implements the ceiling exactly. With original inputs $m_0,n_0$, the [loop invariant](../../../../../loop-invariant.md) is

$$
\frac{m_0}{n_0}=\sum_{0\leq j<e.i}\frac1{e.x[j]}+\frac mn,\qquad 0\leq m<n.
$$

All stored denominators are positive; `e.i` counts precisely the initialized entries. Part (b) makes $m$ a strictly decreasing nonnegative [loop variant](../../../../../loop-variant.md). At termination the residual is zero, so the stored [Egyptian fraction](../../../../../egyptian-fraction.md) has the original value. The promised capacity bound justifies the array assertion. Denominators can grow rapidly, so the integer operations require exact sufficiently large storage.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
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
